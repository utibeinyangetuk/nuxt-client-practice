<template>
	<div class="card">
		<img
			class="image"
			:src="require(`@/assets/${card.image}`)"
			alt="#fire extinguisher"
		/>
		<h3 class="header">
			{{ card.title }}
		</h3>
		<p class="snippet">{{ card.snippet }}</p>
	</div>
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
