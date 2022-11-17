<script>
	import Hamburger from './Hamburger.svelte';
	import Logo from '../Global/Logo.svelte';
	import Nav from './Nav.svelte';
</script>

<header class="header ">
	<Logo text="d" />
	<Nav />
	<Hamburger />
</header>

<style lang="scss">
	.header {
		position: fixed;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0 25px;
		width: 100%;
		height: 6rem;
		transition: all 200ms ease-in-out;

		@media (min-width: 768px) {
			padding: 0 50px;
		}
	}
</style>
