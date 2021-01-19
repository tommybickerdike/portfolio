<script lang="ts">
	import Image from "svelte-image";
</script>

<main>
	<div class="image">
		<Image src="/tommy-bickerdike.png" />
	</div>
	<h1>Machine &amp; Oil is the product design portfolio of <span>Tommy Bickerdike</span></h1>
</main>

<style>
	main {
		padding: 4rem;
		margin: 0 auto;
		min-height: 100vh;
		width: 100%;
		display: flex;
		position: relative;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
	}

	h1 {
		font-weight: inherit;
		position: relative;
		z-index: 2;
	}
	h1 span {
		display: block;
		font-size: 6rem;
		line-height: 1.1;
		font-weight: 700;
	}

	aside {
		display: block;
		margin-top: -1rem;
	}

	.image {
		position: fixed;
		top: 0;
		right: 0;
		height: 600px;
		width: 500px;
		max-width: 100%;
		z-index: 1;
		mix-blend-mode: multiply;
	}

	@media (max-width: 65ch) {
		main {
			padding: 1rem;
			font-size: 13px;
		}
		h1 span {
			font-size: 4rem;
		}
	}
</style>