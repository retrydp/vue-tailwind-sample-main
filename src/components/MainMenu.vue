<script setup lang="ts"></script>

<template>
  <div class="flex w-full shadow-md xl:px-29">
    <div class="flex w-full px-4 py-2">
      <div class="flex items-center w-full gap-5">
        <img class="w-10 h-8" src="../assets/logo.png" alt="" />
        <div class="hidden text-xs font-bold uppercase xl:block">sitename</div>
        <button class="hidden gap-4 p-2 rounded-sm md:flex xl:w-35 bg-lime-600" type="button">
          <div class="flex w-5">
            <img src="../assets/miniMenu.png" alt="" />
          </div>
          <p class="text-base text-white md:hidden xl:flex">Catalog</p>
        </button>
        <div class="relative w-full">
          <img class="absolute right-2 bottom-2" src="../assets/search_icon.svg" alt="" />
          <input
            class="w-full px-4 py-2 border rounded-sm placeholder:text-base/10 border-lime-600"
            type="text"
            placeholder="Find goods"
            id="search"
          />
        </div>
      </div>
    </div>
    <div
      class="fixed bottom-0 flex flex-row justify-between w-full px-4 py-2 grow md:static md:w-94 md:pl-0 xl:px-4"
    >
      <button class="flex flex-col items-center justify-between md:hidden">
        <img class="w-6 h-6" src="../assets/miniMenu.png" alt="" />
        <div class="text-[8px]">Catalog</div>
      </button>
      <button class="flex flex-col items-center justify-between">
        <img class="w-6 h-6" src="../assets/favorite_icon.png" alt="" />
        <div class="text-[8px]">Favorite</div>
      </button>
      <button class="flex flex-col items-center justify-between">
        <img class="w-6 h-6" src="../assets/orders_icon.png" alt="" />
        <div class="text-[8px]">Orders</div>
      </button>
      <button class="flex flex-col items-center justify-between">
        <div class="relative">
          <img class="w-6 h-6" src="../assets/cart_icon.png" alt="" />
          <div
            class="absolute bg-amber-600 rounded-full px-1 text-[8px] text-white bottom-4 right-0"
          >
            1
          </div>
        </div>
        <div class="text-[8px]">Cart</div>
      </button>
      <button class="flex flex-row items-center justify-between gap-2.5">
        <img class="w-10 h-10 rounded-full" src="../assets/avatar.png" alt="" />
          <div class="hidden xl:block">Username</div>
      </button>
    </div>
  </div>
</template>
