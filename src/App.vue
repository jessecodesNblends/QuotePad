<template>
	<div class="container">
		<app-new-quote></app-new-quote>
		<appQuoteGrid v-bind:quotes='quotes'></appQuoteGrid>
	</div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue'
import NewQuote from './components/NewQuote.vue'

export default {
	components: {
		appQuoteGrid: QuoteGrid,
		appNewQuote: NewQuote
	},
	data: function() {
		return {
			quotes: [
				'Just a quote to see something',
			],
			maxQuotes: 10,
		}	
	},
};
</script>
