<script setup lang="ts"></script>
<template>
  <div
    class="fixed bottom-0 flex flex-row justify-between w-full px-4 py-2 md:static md:w-96 md:pl-0 xl:px-4"
  >
    <button class="flex flex-col items-center justify-between md:hidden">
      <img class="w-6 h-6" src="../../assets/miniMenu.png" alt="" />
      <div class="text-[8px]">Catalog</div>
    </button>
    <button class="flex flex-col items-center justify-between">
      <img class="w-6 h-6" src="../../assets/favorite_icon.png" alt="" />
      <div class="text-[8px]">Favorite</div>
    </button>
    <button class="flex flex-col items-center justify-between">
      <img class="w-6 h-6" src="../../assets/orders_icon.png" alt="" />
      <div class="text-[8px]">Orders</div>
    </button>
    <button class="flex flex-col items-center justify-between">
      <div class="relative">
        <img class="w-6 h-6" src="../../assets/cart_icon.png" alt="" />
        <div class="absolute bottom-4 right-0 bg-amber-600 text-white text-[8px] rounded-full px-1">
          1
        </div>
      </div>
      <div class="text-[8px]">Cart</div>
    </button>
    <button class="flex flex-row items-center gap-2.5">
      <img class="w-10 h-10 rounded-full" src="../../assets/avatar.png" alt="" />
      <div class="hidden xl:block">Username 1</div>
    </button>
  </div>
</template>
