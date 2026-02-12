<script setup lang="ts">
import bannerCart from '@assets/banner_cart.png';
import bannerTest from '@assets/banner_test.png';
const promoHighlightsMap = [
  {
    title: 'Promo Highlights Component',
    description: 'Earn points every time you shop — online or in-store.”',
    imageSrc: bannerCart,
    color: 'green',
    altText: 'Cart banner',
    href: '#'
  },
  {
    title: 'Promo Highlights Component',
    description: 'Earn points every time you shop — online or in-store.”',
    imageSrc: bannerTest,
    color: 'orange',
    altText: 'Slogan banner',
    href: '#'
  }
];
const colorMap = {
  green: 'bg-green-100 hover:shadow-green-200',
  orange: 'bg-orange-100 hover:shadow-orange-200'
};
</script>
<template>
  <div class="flex gap-1 flex-col md:flex-row justify-between lg:gap-8 xl:gap-10">
    <a
      v-for="{title, description, imageSrc, color, altText, href} in promoHighlightsMap"
      :key="title"
      :href="href"
      :class="['flex rounded-sm grow items-center hover:shadow-lg', colorMap[color]]"
    >
      <div class="flex flex-col gap-1.5 p-5">
        <p class="font-bold text-xl">{{ title }}</p>
        <p class="">{{ description }}</p>
      </div>
      <img class="block object-scale-down w-1/2 max-h-42" :src="imageSrc" :alt="altText" />
    </a>
  </div>
</template>
