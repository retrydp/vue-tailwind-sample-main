<script setup lang="ts">
import { ProductCardDetails, ProductCardPreview } from './ui';
</script>

<template>
  <div
    class="flex flex-col bg-white rounded-sm shadow-md hover:shadow-xl hover:shadow-def-orange/35"
  >
    <ProductCardPreview />
    <ProductCardDetails />
  </div>
</template>
