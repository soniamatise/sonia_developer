<template>
	<section class="row center small-full medium-half large-20">
		<div class="column">
			<h3 class="text-center" v-html="text" />
		</div>
	</section>
</template>

<script>
export default {
	components: {
	},
	props: ['text']
};
</script>

<style lang="scss">
// @import '~henris';
// .centered-text{
// 	padding-bottom: grid(2.75);
// 	@media #{$small-only} {
// 		padding: 0 32px 80px;
// 	}
// }
</style>