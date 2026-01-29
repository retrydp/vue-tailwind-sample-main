<script setup lang="ts">
  import MenuCatalogButton from './MenuCatalogButton.vue';
  import MenuSearchBar from './MenuSearchBar.vue';
  import MenuNavbarPersonal from './MenuNavbarPersonal.vue';
</script>

<template>
  <div class="flex justify-center w-full shadow-md md:justify-between xl:px-28">
    <div class="flex w-full px-4 py-2">
      <div class="flex items-center w-full gap-5">
        <img class="w-10 h-8 object-contain" src="../../assets/logo.png" alt="" />
        <div class="hidden xl:flex gap-1">
          <p class="font-bitcount font-bold text-lg text-amber-600 xl:block drop-shadow-[0_1.2px_1.2px_rgba(0,0,0,0.4)]">Daily</p>
          <p class="font-bitcount font-bold text-lg text-white xl:block drop-shadow-[0_1.2px_1.2px_rgba(0,0,0,0.7)]">Food</p>
        </div>

        <MenuCatalogButton />
        <MenuSearchBar />
      </div>
    </div>
    <MenuNavbarPersonal />
  </div>
</template>
