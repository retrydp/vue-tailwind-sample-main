<script setup lang="ts">
import ProductCardDetails from './ui/ProductCardDetails.vue';
import ProductCardPreview from './ui/ProductCardPreview.vue';
</script>

<template>
  <div
    class="flex flex-col bg-white rounded-sm shadow-md hover:shadow-xl hover:shadow-def-orange/35"
  >
    <ProductCardPreview />
    <ProductCardDetails />
  </div>
</template>
