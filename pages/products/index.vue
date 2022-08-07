<template>
  <div class="container">
    <LargeCardDisplay v-for="cardInfo in largeCardInfo.slice(0, 1)" :key="cardInfo.id" :cardsSection="cardInfo" />
    <smallCardDisplay v-for="cardInfo in smallCardInfo" :key="cardInfo.id" :cardsSection="cardInfo" />
  </div>
</template>

<script setup>
import { largeCardSections, smallCardSections } from "@/assets/data";
import { ref } from "vue";
const largeCardInfo = ref(largeCardSections);
const smallCardInfo = ref(smallCardSections);
</script>

<style scoped>
</style>
