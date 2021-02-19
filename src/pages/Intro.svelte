<script lang="ts">
	import Image from "svelte-image";
	import { fly, fade } from "svelte/transition";
</script>

<svelte:head>
  <title>Tommy Bickerdike - Intro</title>
</svelte:head>

<section in:fly={{ y: 50, duration: 500 }} out:fly={{ y: 50, duration: 300 }}>
	<h1>Tommy Bickerdike</h1>
	<p>A product designer and creative technologist currently 
		making e-commerce websites as Creative Director of Music Glue.</p>
</section>
<div class="image" in:fade={{ duration: 2000 }} out:fly={{ x: 100, duration: 300 }}>
	<div class="image-process">
		<Image src="images/tommy-bickerdike.jpg" alt="Tommy Bickerdike" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 500px" threshold="0.8"/>
	</div>
</div>

<style>
	h1 {
		font-weight: inherit;
		position: relative;
		display: block;
		font-size: 6rem;
		line-height: 1.1;
		font-weight: 700;
		margin: 0;
	}

	p {
		font-size: 1.5rem;
		width: 50ch;
		max-width: 100%;
	}

	.image {
		position: fixed;
		top: 0;
		right: 0;
		height: 100vh;
		width: 500px;
		max-width: 80%;
		display: flex;
		flex-direction: column;
		justify-content: center;
		z-index: 1;
		background: #262C57;
	}

	.image-process {
		mix-blend-mode: multiply;
	}

	@media (max-width: 65ch) {
		h1 {
			font-size: 4rem;
		}
	}
</style>