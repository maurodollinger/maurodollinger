<template>
  <div>
  	<header-component></header-component>
    <nuxt/>
  </div>
</template>

<script>
    import Header from './header-component.vue';
	export default{
		name: 'app',
		components:{
			'header-component':Header
		}
	}
</script>

<style>
</style>

