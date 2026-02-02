<script setup lang="ts">
import DisplaySection from '../LandingContent/DisplaySection.vue';
import PromoHighlights from '@components/LandingContent/PromoHighlights.vue';
import ProductGrid from '@components/Product/ProductGrid.vue';

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
      title: 'advantages',
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
