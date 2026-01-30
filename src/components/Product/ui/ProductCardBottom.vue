<script setup lang="ts">
import ProductRating from './ProductCardRating.vue';
import ProductAddToCartBtn from './ProductCardAddButton.vue';
</script>

<template>
  <div class="flex flex-col gap-2 p-2 border-amber-300">
    <div class="flex justify-between w-full">
      <div class="flex flex-col justify-between">
        <span class="text-lg font-bold">44,50 $</span>
        <span class="text-xs text-gray-400">Card prize</span>
      </div>
      <div class="flex flex-col justify-between text-right">
        <span>50,50 $</span>
        <span class="text-xs text-gray-400">Common prize</span>
      </div>
    </div>
    <span class="line-clamp-3"
      >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Mollitia aliquid assumenda
      consequatur quidem incidunt modi, sapiente consectetur fugiat vitae deleniti sequi expedita,
      corporis molestias a obcaecati corrupti optio soluta beatae!</span
    >
    <ProductRating :rating="3" />
    <ProductAddToCartBtn />
  </div>
</template>
