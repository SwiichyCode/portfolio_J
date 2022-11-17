<script>
	import Header from '../libs/Header/Header.svelte';
	import Main from '../libs/Main/Main.svelte';
	import SideLink from '../libs/Global/SideSocial.svelte';
	import SideEmail from '../libs/Global/SideEmail.svelte';
</script>

<div class="container">
	<SideLink />
	<SideEmail />
	<Header />
	<Main />
</div>

<style>
	.container {
		width: 100%;
		height: auto;
		transition: all 200ms ease-in-out;
		background-color: #0A192F;
		overflow: hidden;
	}
</style>
