<template>
	<div class="container">
		<appQuoteGrid></appQuoteGrid>
	</div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid'
export default {
	data: function() {
		return {
			quotes: [
				'Just a quote to see something',
			],
			maxQuotes: 10,
		}	
	},
	components: {
		appQuoteGrid: QuoteGrid,
	}
};
</script>
