<template>
	<div class="container">
		<h4 class="header">{{ cardsSection.title }}</h4>
		<p class="snippet">
			{{ cardsSection.snippet }}
		</p>
		<div class="cards-container">
			<LargeCard
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

<style scoped>
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.cards-container {
		display: flex;
		justify-content: space-evenly;
    gap: 20px;
	}
</style>
