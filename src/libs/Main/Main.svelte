<script>
	import HeroSection from './HeroSection.svelte';
</script>

<main>
	<!-- Hero Section -->
	<HeroSection />
</main>

<style lang="scss">
	main {
		margin: 0px auto;
		width: 100%;
		max-width: 1600px;
		min-height: 100vh;
		transition: all 200ms ease-in-out;
		padding: 0 25px;

		@media (min-width: 768px) {
			padding: 0px 140px;
		}
	}
</style>
