<script setup lang="ts">
  const inputGroupStyle = 'flex flex-col gap-2';
  const labelStyle = 'text-xs text-gray-600 font-bold';
  const inputStyle = 'p-4 text-base text-gray-600 border-2 border-slate-400 rounded-lg w-full focus:outline-indigo-500';
</script>
<template>
  <form class="flex  flex-col w-3xl bg-white p-5 md:p-20 gap-8">
    <div :class="inputGroupStyle">
      <label :class="labelStyle" for="username">User name</label>
      <input
        :class="inputStyle"
        type="text"
        name="username"
        id="username"
        placeholder="Enter username"
        required
      />
    </div>
    <div :class="inputGroupStyle">
      <label :class="labelStyle" for="password">Password</label>
      <input
        :class="inputStyle"
        type="password"
        name="password"
        id="password"
        placeholder="Enter password"
        required
      />
    </div>
    <div class="flex justify-end">
      <button class="bg-indigo-500 w-43 h-14 rounded-lg text-white">lol</button>
    </div>
  </form>
</template>
