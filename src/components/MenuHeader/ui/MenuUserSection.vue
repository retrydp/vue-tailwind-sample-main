<script setup lang="ts">
import {
  MenuFavoriteButton,
  MenuUserButton,
  MenuCartButton,
  MenuOrdersButton,
  MenuCatalogSm
} from '.';
</script>
<template>
  <div
    class="fixed bottom-0 flex flex-row justify-between w-full px-4 py-2 bg-white md:static md:w-96 md:pl-0 z-1"
  >
    <MenuCatalogSm />
    <MenuFavoriteButton />
    <MenuOrdersButton />
    <MenuCartButton />
    <MenuUserButton />
  </div>
</template>
