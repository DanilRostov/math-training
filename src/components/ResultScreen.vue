<template>
	<div class="alert alert-primary">
		<h3>Попал в цель: {{ stats.success }}</h3>
		<h3>Ошибся: {{ stats.error }}</h3>
		<hr>
		<button class="btn btn-primary" @click="$emit('repeat')">Го сначала</button>
		<button class="btn btn-primary" @click="$emit('nextLevel')">Следующий уровень</button>
	</div>
</template>

<script>
	export default {
		props: ['stats']
	}
</script>

<style>
	
</style>