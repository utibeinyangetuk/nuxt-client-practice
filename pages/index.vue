<template>
  <div class="container">
    <navbar />
    <hero />
    <largeCardDisplay v-for="cardInfo in LargeCardInfo" :key="cardInfo.id" :cardsSection="cardInfo" />
    <smallCardDisplay v-for="cardInfo in smallCardSection" :key="cardInfo.id" :cardsSection="cardInfo" />
  </div>
</template>

<script setup>
import { largeCardSections, smallCardSections } from '@/assets/data';
import { ref } from 'vue';
const LargeCardInfo = ref(largeCardSections)
const smallCardSection = ref(smallCardSections)
</script>
