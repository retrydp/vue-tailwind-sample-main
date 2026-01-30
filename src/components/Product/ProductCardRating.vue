<script setup lang="ts">
import { computed, PropType } from 'vue';

const { rating = 1 } = defineProps({
  rating: Number as PropType<1 | 2 | 3 | 4 | 5>
});

const STARS_MAX = 5;
const STAR_IMAGE_COLORS = ['#BFBFBF', '#FF6633'];

const colors = computed(() =>
  Array.from({ length: STARS_MAX }, (_, idx) => STAR_IMAGE_COLORS[idx < rating ? 1 : 0])
);
</script>
<template>
  <div class="flex flex-row gap-1">
    <svg
      v-for="(color, idx) in colors"
      :key="idx"
      width="16"
      height="16"
      viewBox="0 0 13 13"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M5.5642 0.557219C5.93102 -0.186027 6.99086 -0.186025 7.35767 0.55722L8.57941 3.03273C8.72507 3.32787 9.00664 3.53244 9.33235 3.57977L12.0642 3.97673C12.8844 4.09592 13.212 5.10389 12.6184 5.68243L10.6416 7.60934C10.4059 7.83907 10.2984 8.17007 10.354 8.49447L10.8207 11.2153C10.9608 12.0322 10.1034 12.6552 9.36975 12.2695L6.92628 10.9849C6.63495 10.8317 6.28692 10.8317 5.9956 10.9849L3.55213 12.2695C2.8185 12.6552 1.96107 12.0322 2.10118 11.2153L2.56784 8.49447C2.62348 8.17007 2.51593 7.83907 2.28024 7.60934L0.303434 5.68242C-0.290083 5.10389 0.037428 4.09592 0.857648 3.97673L3.58953 3.57977C3.91524 3.53244 4.19681 3.32787 4.34247 3.03272L5.5642 0.557219Z"
        :fill="color"
      />
    </svg>
  </div>
</template>
