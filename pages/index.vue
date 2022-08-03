<template>
	<div class="container">
		<hero />
		<largeCardDisplay
			v-for="cardInfo in LargeCardInfo"
			:key="cardInfo.id"
			:cardsSection="cardInfo"
		/>
		<smallCardDisplay
			v-for="cardInfo in smallCardSection"
			:key="cardInfo.id"
			:cardsSection="cardInfo"
		/>
	</div>
</template>

<script setup>
	import { ref } from 'vue'
	import { largeCardSections, smallCardSections } from '@/assets/data'
	const LargeCardInfo = ref(largeCardSections)
	const smallCardSection = ref(smallCardSections)
</script>
