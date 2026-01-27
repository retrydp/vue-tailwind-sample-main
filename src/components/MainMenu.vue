<template>
  <div class="flex justify-center w-full shadow-md md:justify-between xl:px-28">
    <div class="flex w-full px-4 py-2">
      <div class="flex items-center w-full gap-5">
        <img class="w-10 h-8" src="../assets/logo.png" alt="" />
        <div class="hidden text-xs font-bold uppercase xl:block">sitename</div>
        <button class="hidden gap-4 p-2 rounded-sm md:flex xl:w-36 bg-lime-600" type="button">
          <div class="flex w-5">
            <img src="../assets/miniMenu.png" alt="" />
          </div>
          <p class="hidden text-base text-white xl:flex">Catalog</p>
        </button>
        <div class="relative w-full">
          <img class="absolute right-2 bottom-2" src="../assets/search_icon.svg" alt="" />
          <input
            class="w-full px-4 py-2 border rounded-sm border-lime-600 placeholder:text-base/10"
            type="text"
            placeholder="Find goods"
            id="search"
          />
        </div>
      </div>
    </div>
    <div
      class="fixed bottom-0 flex flex-row justify-between w-full px-4 py-2 md:static md:w-96 md:pl-0 xl:px-4"
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
            class="absolute bottom-4 right-0 bg-amber-600 text-white text-[8px] rounded-full px-1"
          >
            1
          </div>
        </div>
        <div class="text-[8px]">Cart</div>
      </button>
      <button class="flex flex-row items-center gap-2.5">
        <img class="w-10 h-10 rounded-full" src="../assets/avatar.png" alt="" />
        <div class="hidden xl:block">Username 1</div>
      </button>
    </div>
  </div>
</template>
