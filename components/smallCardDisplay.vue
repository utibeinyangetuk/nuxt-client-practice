<template>
	<div class="container">
		<h3 class="header">{{ props.cardsSection.title }}</h3>
		<div class="card-container">
			<smallCard
				v-for="card in cardsSection.cards"
				:key="card.id"
				:card="card"
			/>
		</div>
	</div>
</template>

<script setup>
const props = defineProps(['cardsSection'])
</script>

<style scoped></style>
