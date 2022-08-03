<template>
	<div class="card-container">
		<img
			class="image"
			:src="require(`@/assets/${card.image}`)"
			alt="extinguisher image"
		/>
	</div>
</template>

<script setup>
const props = defineProps(['card'])
</script>

<style scoped>
.card-container {
	border: 1px solid;
	padding: 10px;
	width: 400px;
	border-radius: 10px;
}

.image {
	width: 100%;
}
</style>
