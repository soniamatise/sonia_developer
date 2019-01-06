<template>
	<main class="page page--home">
		<intro-text text="Creative Developer based in Amsterdam. The synthesis of code and design is the best way of expressing my own art next to music." />
		<section-container title="work" information="blablabla">
			<work-block
				:image="patricionusselder"
				url="http://patricionusselder.nl/"
				title="test hello hello"
				description="Lorem Ipsum is slechts een proeftekst uit het drukkerij- en zetterijwezen. Lorem Ipsum is de standaard proeftekst in deze bedrijfstak sinds de 16e eeuw, toen een onbekende drukker een zethaak met letters."
			/>
			<work-block :image="ictsolve" title="test hello hello" />
			<work-block :image="wereldvrede" title="test hello hello" />
			<work-block :image="soniaanubis" title="test hello hello" />
			<work-block :image="aangenaam" title="test hello hello" />
			<work-block :image="nielsonair" title="test hello hello" />
		</section-container>
		<full-text
			text="<p>Interested In working with me or have a project in mind?<br>
				Feel free to <strong>write me</strong>, I’ll be happy to <strong>get back</strong> to you. Or not.</p>"
		/>
	</main>
</template>

<script>
import IntroText from '~/components/sections/intro-text.vue';
import FullText from '~/components/sections/full-text.vue';
import SectionContainer from '~/components/sections/section-container.vue';
import WorkBlock from '~/components/reusable/work-block.vue';


export default {
	components: {
		IntroText,
		SectionContainer,
		WorkBlock,
		FullText
	},
	data(){
		return {
			patricionusselder: require('~/static/images/projects/patricionusselder.png'),
			ictsolve: require('~/static/images/projects/ictsolve.jpg'),
			nielsonair: require('~/static/images/projects/nielsonair.jpg'),
			aangenaam: require('~/static/images/projects/aangenaaminbusiness.jpg'),
			wereldvrede: require('~/static/images/projects/wereldvrede.jpg'),
			soniaanubis: require('~/static/images/projects/soniaanubis.jpg'),
		};
	},
};
</script>

<style lang="scss">
@import '~tools';

.page {
	// general page styles
	&--home {
		// specific home styles
	}
}

</style>
