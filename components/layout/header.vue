<template>
	<header id="header" class="header">
		<div class="row center small-full medium-full large-20">
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
	</header>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import '~tools';

.header {
	// Header styles
}
</style>
