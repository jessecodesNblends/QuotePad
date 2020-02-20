<template>
	<div class="container">
		<app-header></app-header>
		<app-new-quote v-on:quoteAdded='newQuote'></app-new-quote>
		<appQuoteGrid v-bind:quotes='quotes' v-on:quoteDeleted='deleteQuote'></appQuoteGrid>
		<div class="row">
			<div class="col-sm-12 text-center">
				<div class="alert alert-info">Attention!: Select a Quote to delete</div>
			</div>
		</div>
	</div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue'
import NewQuote from './components/NewQuote.vue'
import Header from './components/Header.vue'

export default {
	components: {
		appQuoteGrid: QuoteGrid,
		appNewQuote: NewQuote,
		appHeader: Header,
	},
	data: function() {
		return {
			quotes: [
				'Just a quote to see something',
			],
			maxQuotes: 10,
		}	
	},
	methods: {
		newQuote(quote) {
			this.quotes.push(quote);
		},
		deleteQuote(index) {
			this.quotes.splice(index, 1)
		}
	}
};
</script>
