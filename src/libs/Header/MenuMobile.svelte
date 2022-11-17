<script>
	import { fly } from 'svelte/transition';
	const flyParams = {
		x: window.innerWidth,
		duration: 500
	};

	const items = [
		{ text: 'About', href: '#' },
		{ text: 'Experience', href: '#' },
		{ text: 'Work', href: '#' },
		{ text: 'Contact', href: '#' }
	];
</script>

<div class="mobile-menu" transition:fly={flyParams}>
	<div class="mobile-menu-wrapper ">
		<ul>
			{#each items as { text, href }, index}
				<li>
					<a {href}
						><span class="nav-index">0{index + 1}.</span>
						<span class="nav-text">{text}</span>
					</a>
				</li>
			{/each}
		</ul>
	</div>
</div>

<style lang="scss">
	.mobile-menu {
		position: absolute;
		top: 0;
		right: 0;
		width: 100%;
		height: 100vh;
		font-family: SF Mono Medium;

		@media (min-width: 768px) {
			display: none;
		}

		&-wrapper {
			position: absolute;
			top: 0;
			right: 0;
			display: flex;
			justify-content: center;
			width: 75%;
			height: 100%;
			padding-top: 15rem;
			background: #112240;

			ul {
				display: flex;
				flex-direction: column;
				gap: 2rem;

				a {
					display: flex;
					flex-direction: column;
					align-items: center;

					.nav-index {
						color: #64ffda;

						font-size: 0.875rem;
						line-height: 1.25rem;
					}
					.nav-text {
						color: #b8c2e2;
						font-size: 1.125rem;
						line-height: 1.75rem;
					}
				}
			}
		}
	}
	.mobile-menu::after {
		content: '';
		position: absolute;
		width: 25%;
		height: 100vh;
		background: transparent;
		backdrop-filter: blur(4px);
	}
</style>
