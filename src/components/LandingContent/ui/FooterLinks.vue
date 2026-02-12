<script setup lang="ts">
const linksMap = [
  { name: 'About', href: '#' },
  { name: 'Contacts', href: '#' },
  { name: 'Articles', href: '#' },
  { name: 'Job vacancy', href: '#' },
  { name: 'Personal data processing policy', href: '#' }
];
</script>
<template>
  <div class="flex gap-4 flex-wrap text-xs items-center md:grow">
    <a
      class="hover:text-def-orange lg:text-lg"
      v-for="link in linksMap"
      :key="link.name"
      :href="link.href"
      >{{ link.name }}</a
    >
  </div>
</template>
