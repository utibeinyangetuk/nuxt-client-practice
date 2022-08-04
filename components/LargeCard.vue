<template>
  <Nuxt-Link :to="`/products/${card.id}`" class="card">
    <img class="image" :src="require(`@/assets/images/${card.image}`)" alt="#fire extinguisher" />
    <h3 class="header">
      {{ props.card.title }}
    </h3>
    <p class="snippet">{{ props.card.snippet }}</p>
  </Nuxt-Link>
</template>

<script setup>
const props = defineProps(['card'])
</script>

<style scoped>
.card {
  border: 1px solid;
  padding: 10px;
  width: 400px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.image {
  border: 1px solid;
  width: 100%;
}
</style>
