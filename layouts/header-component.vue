<template>
	<header>
		<nav id="navigation" class="container">
			<ul>
				<li><a href="#" v-scroll-to="'#skills'">Skills</a></li>
				<li><a href="#" v-scroll-to="'#abilities'">Ability</a></li>
				<li><a href="#" v-scroll-to="'#contact'">Contact</a></li>
			</ul>
		</nav>
	</header><!-- /header -->
</template>

<script>
	export default{
		name:'Header'
	}
</script>