<script setup lang="ts">
import ProductCardBottom from './ui/ProductCardBottom.vue';
import ProductCardTop from './ui/ProductCardTop.vue';
</script>

<template>
  <div
    class="flex flex-col bg-white rounded-sm shadow-md hover:shadow-xl hover:shadow-def-orange/35"
  >
    <ProductCardTop />
    <ProductCardBottom />
  </div>
</template>
