<template>
	<div>
		<h3>i am product id {{ products }}</h3>
	</div>
</template>

<script>
export default {
	computed: {
		products() {
			return this.$store.getters.getProductsById(this.$route.params.id)
		},
	},
}
</script>

<style scoped></style>
