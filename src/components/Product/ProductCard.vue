<script setup lang="ts">
  import ProductCardBottom from './ProductCardBottom.vue';
  import ProductCardTop from './ProductCardTop.vue';
</script>

<template>
  <div
    class="flex flex-col rounded-sm bg-white shadow-md hover:shadow-xl hover:shadow-amber-600/35"
  >
    <ProductCardTop />
    <ProductCardBottom />
  </div>
</template>
