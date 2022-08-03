<template>
	<div>
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

<style scoped></style>
