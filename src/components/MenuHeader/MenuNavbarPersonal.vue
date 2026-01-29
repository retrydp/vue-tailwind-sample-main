<script setup lang="ts">
  import MenuCartButton from './MenuCartButton.vue';
  import MenuUserButton from './MenuUserButton.vue';
</script>
<template>
  <div
    class="fixed bottom-0 flex flex-row justify-between w-full px-4 py-2 bg-white md:static md:w-96 md:pl-0 z-1"
  >
    <button class="flex flex-col items-center justify-between md:hidden">
      <img class="w-6 h-6" src="../../assets/miniMenu.png" alt="" />
      <div class="text-[8px] md:text-xs">Catalog</div>
    </button>
    <button class="flex flex-col items-center justify-between">
      <img class="w-6 h-6" src="../../assets/favorite_icon.png" alt="" />
      <div class="text-[8px] md:text-xs">Favorite</div>
    </button>
    <button class="flex flex-col items-center justify-between">
      <img class="w-6 h-6" src="../../assets/orders_icon.png" alt="" />
      <div class="text-[8px] md:text-xs">Orders</div>
    </button>
    <MenuCartButton />
    <MenuUserButton />
  </div>
</template>
