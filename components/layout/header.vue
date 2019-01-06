<template>
	<header id="header" class="header">
		<div class="row center small-full medium-full large-12">
			<div class="column">
				<nav class="main-nav">
					<ul class="main-nav__list">
						<li class="main-nav__item">
							<nuxt-link to="/work" class="main-nav__link">
								<span class="main-nav__text">Work</span>
							</nuxt-link>
						</li>
						<li class="main-nav__item">
							<nuxt-link to="/" class="main-nav__link">
								<span class="main-nav__text"><h1>Sonia Nusselder</h1></span>
							</nuxt-link>
						</li>
						<li class="main-nav__item">
							<nuxt-link to="/contact" class="main-nav__link">
								<span class="main-nav__text">Contact</span>
							</nuxt-link>
						</li>
					</ul>
				</nav>
			</div>
		</div>
		<contact-section/>
	</header>
</template>

<script>
import ContactSection from '~/components/sections/contact-section.vue';

export default {
	components: {
		ContactSection,
	}
};
</script>

<style lang="scss">
@import '~tools';

.header {
	padding: 2rem 0;
	.main-nav {
		&__list {
			display: flex;
			flex-direction: row;
			justify-content: space-around;
			align-items: center;
		}
	}
}
</style>
