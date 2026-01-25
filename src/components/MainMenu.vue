<script setup lang="ts"></script>

<template>
  <div class="flex w-full shadow-md xl:px-29">
    <div class="flex py-2 px-4 w-full">
      <div class="flex items-center gap-5 w-full">
        <img class="w-10 h-8" src="../assets/logo.png" alt="" />

       <div class="hidden xl:block text-xs uppercase font-bold">sitename</div>
        <div class="w-10 hidden md:block bg-lime-600 p-2 rounded-sm">
          <img src="../assets/miniMenu.png" alt="" />
        </div>
        <div class="w-full relative">
          <img class="absolute right-2 bottom-2" src="../assets/search_icon.svg" alt="" />
          <input
            class="px-4 py-2 w-full placeholder:text-base/10 border rounded-sm border-lime-600"
            type="text"
            placeholder="Find goods"
            id="search"
          />
        </div>
      </div>
    </div>
    <div class="flex flex-row justify-between w-full fixed md:static md:w-94 bottom-0 px-4 py-2 md:pl-0 xl:px-4">
      <div class="flex flex-col items-center justify-between md:hidden">
        <img class="w-6 h-6" src="../assets/miniMenu.png" alt="" />
        <div class="text-[8px]">Catalog</div>
      </div>
      <div class="flex flex-col items-center justify-between">
        <img class="w-6 h-6" src="../assets/favorite_icon.png" alt="" />
        <div class="text-[8px]">Favorite</div>
      </div>
      <div class="flex flex-col items-center justify-between">
        <img class="w-6 h-6" src="../assets/orders_icon.png" alt="" />
        <div class="text-[8px]">Orders</div>
      </div>
      <div class="flex flex-col items-center justify-between">
        <div class="relative">
          <img class="w-6 h-6" src="../assets/cart_icon.png" alt="" />
          <div
            class="absolute bg-amber-600 rounded-full px-1 text-[8px] text-white bottom-4 right-0"
          >
            1
          </div>
        </div>

        <div class="text-[8px]">Cart</div>
      </div>
      <div class="flex flex-col items-center justify-between">
        <img class="w-10 h-10 rounded-full" src="../assets/avatar.png" alt="" />
      </div>
    </div>
  </div>
</template>
