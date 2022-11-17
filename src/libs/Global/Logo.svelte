<script>
	export let text;
</script>

<div class="logo" tabindex="-1">
	<a href="/" aria-label="home"
		><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 84 96"
			><title>Logo</title><g transform="translate(-8.000000, -2.000000)"
				><g transform="translate(11.000000, 5.000000)"
					><polygon
						id="Shape"
						stroke="currentColor"
						stroke-width="5"
						stroke-linecap="round"
						stroke-linejoin="round"
						points="39 0 0 22 0 67 39 90 78 68 78 23"
					/></g
				></g
			></svg
		></a
	>
	<span>{text}</span>
</div>

<style lang="scss">
	.logo {
		position: relative;
		display: flex;
		align-items: center;
		justify-content: center;
		width: 2.5rem;
		z-index: 20;

		& svg {
			width: 2.25rem;
			fill: none;
			color: #64ffda;

			&:hover {
				fill: rgb(100 255 218 / 0.05);
			}
		}

		span {
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			color: #64ffda;
			font-size: 1.125rem;
			line-height: none;
			font-weight: 700;
			text-transform: uppercase;
		}
	}
</style>
