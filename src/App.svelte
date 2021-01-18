<script lang="ts">
	export let name: string;
</script>

<main>
	<h1>Machine &amp; Oil is the product design portfolio of <span>{name}</span></h1>
</main>

<style>
	main {
		padding: 4rem;
		margin: 0 auto;
		min-height: 100vh;
		width: 100%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
	}

	h1 {
		font-weight: inherit;
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