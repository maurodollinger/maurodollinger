<template>
  <div>
  	<header-component></header-component>
    <nuxt/>
    <footer-component></footer-component>
  </div>
</template>

<script>
    import Header from './header-component.vue';
    import Footer from './footer-component.vue';
	export default{
		name: 'app',
		components:{
			'header-component':Header,
			'footer-component':Footer
		}
	}
</script>

<style>
</style>

