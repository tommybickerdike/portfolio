<script lang="ts">
	import Image from "svelte-image";
	import { fly, fade } from "svelte/transition";
</script>

<svelte:head>
  <title>Tommy Bickerdike - Intro</title>
</svelte:head>

<section in:fly={{ y: 50, duration: 500 }} out:fly={{ y: 50, duration: 300 }}>
	<h1>Tommy Bickerdike</h1>
	<p>Product designer and creative technologist.</p>
</section>
<div class="image" in:fade={{ duration: 2000 }} out:fly={{ x: 100, duration: 300 }}>
	<Image wrapperClass="image-wrap" src="images/tommy-bickerdike.jpg" alt="Tommy Bickerdike" width="600" sizes="(max-width: 600px) 80vw, 500px" threshold="0.8"/>
</div>

<style>
	h1 {
		font-weight: inherit;
		position: relative;
		display: block;
		font-size: 6rem;
		padding-top: 10vh;
		line-height: 1.1;
		font-weight: 700;
		margin: 0;
	}

	p {
		font-size: 1.5rem;
		width: 50ch;
		max-width: 100%;
	}

	@media (max-width: 65ch) {
		h1 {
			font-size: 4rem;
		}
	}
</style>
