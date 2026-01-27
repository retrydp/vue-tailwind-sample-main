<script setup lang="ts">
  import CatalogButton from './CatalogButton.vue';
  import Search from './Search.vue';
  import UserMenu from './UserMenu.vue';
</script>

<template>
  <div class="flex justify-center w-full shadow-md md:justify-between xl:px-28">
    <div class="flex w-full px-4 py-2">
      <div class="flex items-center w-full gap-5">
        <img class="w-10 h-8" src="../../assets/logo.png" alt="" />
        <div class="hidden text-xs font-bold uppercase xl:block">sitename</div>
        <CatalogButton />
        <Search />
      </div>
    </div>
    <UserMenu />
  </div>
</template>
