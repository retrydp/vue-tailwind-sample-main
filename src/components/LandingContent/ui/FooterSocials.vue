<script setup lang="ts">
import { FacebookIcon, TwitterIcon, LinkedInIcon, InstagramIcon } from './index';
const socialsMap = [
  {
    name: 'InstagramIcon',
    icon: InstagramIcon,
    href: '#'
  },
  {
    name: 'Facebook',
    icon: FacebookIcon,
    href: '#'
  },
  {
    name: 'LinkedIn',
    icon: LinkedInIcon,
    href: '#'
  },
  {
    name: 'Twitter',
    icon: TwitterIcon,
    href: '#'
  }
];
</script>
<template>
  <div
    class="flex justify-evenly md:flex-wrap md:justify-center md:gap-y-3 xl:flex-nowrap xl:gap-4"
  >
    <a v-for="social in socialsMap" :key="social.name" :href="social.href" class="md:basis-1/2">
      <component :is="social.icon" class="h-5 w-5"
    /></a>
  </div>
</template>
