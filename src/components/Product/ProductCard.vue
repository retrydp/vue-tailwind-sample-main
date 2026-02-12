<script setup lang="ts">
import { ProductCardDetails, ProductCardPreview } from './ui';
</script>

<template>
  <div
    class="flex flex-col bg-white rounded-sm shadow-md hover:shadow-xl hover:shadow-def-orange/35 transition-shadow duration-300"
  >
    <ProductCardPreview />
    <ProductCardDetails />
  </div>
</template>
