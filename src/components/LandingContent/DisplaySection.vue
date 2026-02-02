<script setup lang="ts">
const { title, subLink } = defineProps<{
  title: string;
  subLink: string;
}>();
</script>

<template>
  <div class="flex flex-col">
    <div class="flex justify-between mb-6 items-end">
      <p class="text-2xl text-wrap font-bold">{{ title }}</p>
      <div class="flex gap-7 items-center">
        <p>{{ subLink }}</p>
        <svg class="h-8" focusable="false" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path fill="#afafaf" d="M8.59 16.59L13.17 12 8.59 7.41 10 6l6 6-6 6-1.41-1.41z"></path>
        </svg>
      </div>
    </div>
    <slot></slot>
  </div>
</template>
