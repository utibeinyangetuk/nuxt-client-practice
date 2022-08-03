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

<style scoped>
.card-container{
	display: grid;
		grid-template-columns: repeat(4, 1fr);
		gap: 10px;
		grid-auto-rows: minmax(100px, auto);

}

</style>
