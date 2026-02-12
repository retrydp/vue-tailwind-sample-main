<script setup lang="ts">
import bannerCart from '@assets/banner_cart.png';
import bannerTest from '@assets/banner_test.png';
const promoHighlightsMap = [
  {
    title: 'Promo Highlights Component',
    description: 'Earn points every time you shop — online or in-store.”',
    imageSrc: bannerCart,
    bgColor: 'bg-green-100',
    alt: 'Cart banner'
  },
  {
    title: 'Promo Highlights Component',
    description: 'Earn points every time you shop — online or in-store.”',
    imageSrc: bannerTest,
    bgColor: 'bg-orange-100',
    alt: 'Slogan banner'
  }
];
</script>
<template>
  <div class="flex gap-1 flex-col md:flex-row justify-between lg:gap-8 xl:gap-10">
    <div
      v-for="promo in promoHighlightsMap"
      :key="promo.title"
      :class="['flex rounded-sm grow items-center', promo.bgColor]"
    >
      <div class="flex flex-col gap-1.5 p-5">
        <p class="font-bold text-xl">{{ promo.title }}</p>
        <p class="">{{ promo.description }}</p>
      </div>
      <img class="block object-scale-down w-1/2 max-h-42" :src="promo.imageSrc" :alt="promo.alt" />
    </div>
  </div>
</template>
