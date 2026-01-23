<script setup lang="ts">
  const inputGroupStyle = 'flex flex-col gap-2';
  const labelStyle = 'text-xs text-gray-600 font-bold';
  const inputStyle =
    'p-4 text-base text-gray-600 border-2 border-slate-400 rounded-lg w-full focus:outline-indigo-500';
  const setInputAttrs = (placeholder: string) => ({
    class: inputStyle,
    placeholder,
    required: true,
  });
</script>

<template>
  <form class="flex flex-col w-3xl bg-white p-5 md:p-20 gap-8 rounded-lg">
    <div :class="inputGroupStyle">
      <label :class="labelStyle" for="username">User name</label>
      <input :="setInputAttrs('User name')" name="username" id="username" type="text" />
    </div>
    <div :class="inputGroupStyle">
      <label :class="labelStyle" for="password">Password</label>
      <input :="setInputAttrs('Enter password')" name="password" id="password" type="password" />
    </div>
    <div class="flex justify-end">
      <button class="bg-indigo-500 w-43 h-14 rounded-lg text-white">Submit</button>
    </div>
  </form>
</template>
