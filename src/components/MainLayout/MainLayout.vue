<script setup lang="ts">
import { PromoHighlights, DisplaySection } from '@components/LandingContent';
import { ProductGrid } from '@components/Product';

const sections = [
  {
    component: ProductGrid,
    props: {
      title: 'Featured Products',
      subLink: 'placeholder2'
    }
  },
  {
    component: PromoHighlights,
    props: {
      title: 'Advantages',
      subLink: 'placeholder2'
    }
  }
];
</script>

<template>
  <div class="flex flex-col gap-20 px-3 pb-14 md:px-4 xl:px-28 bg-amber-50 pt-14">
    <DisplaySection v-for="section in sections" :key="section.props.title" v-bind="section.props">
      <component :is="section.component" />
    </DisplaySection>
  </div>
</template>
