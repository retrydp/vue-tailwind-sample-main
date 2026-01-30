<script setup lang="ts">
import MenuCatalogButton from './MenuCatalogButton.vue';
import MenuSearchBar from './MenuSearchBar.vue';
import MenuNavbarPersonal from './MenuNavbarPersonal.vue';
</script>

<template>
  <div class="fixed flex justify-center w-full shadow-md md:justify-between xl:px-28 bg-white z-10">
    <div class="flex w-full px-4 py-2">
      <div class="flex items-center w-full gap-5">
        <img class="object-contain w-10 h-8" src="../../assets/logo.png" alt="" />
        <div class="hidden gap-1 xl:flex">
          <p
            class="font-bitcount font-bold text-lg text-def-orange xl:block drop-shadow-[0_1.2px_1.2px_rgba(0,0,0,0.4)] selection:bg-gray-300"
          >
            Daily
          </p>
          <p
            class="font-bitcount font-bold text-lg text-white xl:block drop-shadow-[0_1.2px_1.2px_rgba(0,0,0,0.7)] selection:bg-def-orange"
          >
            Food
          </p>
        </div>

        <MenuCatalogButton />
        <MenuSearchBar />
      </div>
    </div>
    <MenuNavbarPersonal />
  </div>
</template>
