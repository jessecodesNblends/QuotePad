<template>
	<div>
		<app-quote quote='A wonderful quote'></app-quote>
	</div>
</template>

<script>
import Quote from './components/Quote.vue'
export default {
	components: {
		'app-quote': Quote,
	}
}
</script>
