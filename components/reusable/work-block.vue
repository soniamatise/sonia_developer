<template>
	<article class="work-block">
		<a target="_blank" :href="url">
			<div class="work-block__mask">
				<div :style="`background-image: url('${ image }')`" class="work-block__image" />
			</div>
			<div class="work-block__title">
				<h2>{{ title }}</h2>
				<p>{{ description }}</p>
				<i class="arrow-right"/>
			</div>
		</a>
	</article>
</template>

<script>
export default {
	components: {
	},
	props: ['type', 'title', 'description', 'image', 'url'],
};
</script>
3
<style lang="scss">
@import '~tools';
.work-block {
	transition: width 1s ease 1s;
	position: relative;
	height: grid(8);
	width: 100%;
	cursor: pointer;

	// mask clippath
	&__mask {
		transition: clip-path 0.5s ease-in-out 0.5s, width 1s ease 1s;
		width: 100%;
		height: 100%;
		-webkit-clip-path: polygon(0 0, 80% 0%, 37% 100%, 0% 100%);
		clip-path: polygon(0 0, 80% 0%, 37% 100%, 0% 100%);
	}
	&__image{
		// transition: width 1s ease 1s;
		width: 100%;
		height: 100%;
		background-repeat: no-repeat;
		background-position: center center;
		background-size: cover;
	}
	&__title {
		transition: transform 1s ease 1s;
		position: absolute;
		z-index: 1;
		width: grid(8);
		transform: translate(50%, -50%);
		top: 50%;
		right: 30%;
	}
}
// HOVER STATES
.work-block {
	&:hover {
		width: 50%;
		.work-block__mask {
			-webkit-clip-path: polygon(0 0, 100% 0%, 100% 100%, 0% 100%);
			clip-path: polygon(0 0, 100% 0%, 100% 100%, 0% 100%);
		}
		.work-block__title {
			transform: translate(170%, -50%);
		}
	}
}
</style>
