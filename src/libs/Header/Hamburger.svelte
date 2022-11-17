<script>
	import MdClose from 'svelte-icons/md/MdClose.svelte';
	import '../../styles/icon.css';
	import MobileMenu from './MenuMobile.svelte';

	let active = false;
	const handleClick = () => {
		active = !active;
	};
</script>

<!-- Hamburger BTN-->
{#if !active}
	<button aria-label="menu" class="hamburger-btn" on:click={handleClick}>
		<div class="ham-box">
			<div class="ham-box-inner" />
		</div>
	</button>
{:else}
	<button on:click={handleClick} class="close-btn">
		<MdClose />
	</button>
{/if}

<!-- Mobile Menu-->
{#if active}
	<MobileMenu />
{/if}

<style lang="scss">
	.hamburger-btn,
	.close-btn {
		position: relative;
		display: flex;
		align-items: center;
		justify-content: center;
		width: 2.5rem /* 40px */;
		background: transparent;
		border: none;
		z-index: 20;
		color: #64ffda;

		@media (min-width: 768px) {
			display: none;
		}
	}

	.ham-box {
		position: relative;
		display: inline-block;
		width: 2rem /* 32px */;
		height: 1.5rem /* 24px */;

		.ham-box-inner {
			position: absolute;
			top: 50%;
			right: 0;
			width: 2rem /* 32px */;
			height: 2px;
			border-radius: 0.25rem /* 4px */;
			background-color: #64ffda;
		}
	}
</style>
