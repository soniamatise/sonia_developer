<template>
	<section class="contact__overlay">
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

.contact {
	&__overlay {
		position: fixed;
		transform: translate(-50%, -50%);
		left: 50%;
		top: 50%;
		z-index: 2;
		background-color: color(White);
		width: grid(22);
		height: 80%;
	}
}

// .section {
// 	width: 100%;
// 	height: auto;
// 	&--work {
// 		display: flex;
// 		flex-wrap: wrap;
// 	}
// }
</style>