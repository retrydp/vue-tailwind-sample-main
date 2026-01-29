<script setup lang="ts">
  import { computed, PropType } from 'vue';

  const { rating = 1 } = defineProps({
    rating: Number as PropType<1 | 2 | 3 | 4 | 5>,
  });

  const STARS_MAX = 5;
  const STAR_IMAGE_URLS = [
    new URL('../../assets/plain_star_inactive.svg', import.meta.url).href,
    new URL('../../assets/plain_star.svg', import.meta.url).href,
  ];

  const stars = computed(() =>
    Array.from({ length: STARS_MAX }, (_, idx) => ({
      image: STAR_IMAGE_URLS[idx < rating ? 1 : 0],
    })),
  );
</script>
<template>
  <div class="flex flex-row gap-1">
    <img width="16" height="16" v-for="(star, idx) in stars" :key="idx" :src="star.image" />
  </div>
</template>
