<template>
  <Nuxt-link :to="`/products/${card.id}`" class="card-container">
    <img class="image" :src="require(`@/assets/images/${card.image}`)" alt="extinguisher image" />
  </Nuxt-link>
</template>

<script setup>
const props = defineProps(["card"]);
</script>

<style scoped>
.card-container {
  border: 1px solid;
  padding: 10px;
  border-radius: 10px;
  width: 400px;
}

.image {
  height: 100%;
  width: 100%;
}
</style>
