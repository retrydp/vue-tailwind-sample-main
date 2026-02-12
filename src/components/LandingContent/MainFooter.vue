<script setup lang="ts">
import { FooterSocials, FooterPhone, FooterLinks } from '@components/LandingContent/ui';
</script>
<template>
  <div
    class="flex px-7 gap-10 xl:px-28 md:px-4 md:py-8 pt-10 pb-7 mb-14 md:mb-0 md:flex-nowrap bg-amber-100/80 justify-between flex-wrap bg-[url('@assets/footer_pattern.png')]"
  >
    <img src="@assets/logo.png" alt="Logo" class="max-h-16 block object-contain" />
    <div class="flex flex-col md:flex-row justify-between md:order-last md:items-center md:gap-6">
      <FooterSocials />
      <FooterPhone />
    </div>
    <FooterLinks />
  </div>
</template>
