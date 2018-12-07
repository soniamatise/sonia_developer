<template>
	<section class="row center centered-text small-full medium-full large-full">
		<div class="column">
			<h2>{{ title }}</h2>
			<h4>{{ information }}</h4>
			<div :class="`section section--${ title }`">
				<slot />
			</div>
		</div>
	</section>
</template>

<script>
export default {
	components: {
	},
	props: ['title', 'information']
};
</script>

<style lang="scss">
@import '~tools';


.section {
	width: 100%;
	height: auto;
	&--work {
		display: flex;
		flex-wrap: wrap;
	}
}
</style>