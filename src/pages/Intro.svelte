<svelte:head>
  <title>Tommy Bickerdike</title>
</svelte:head>

<script>
	import Image from "svelte-image";
	import { fly, fade } from "svelte/transition";
</script>

<section in:fly={{ x: -300, duration: 1000 }} out:fade={{ duration: 300 }}>
	<h1>Tommy Bickerdike</h1>
	<p>A senior UX designer and front end developer currently working in e-commerece at Music Glue.</p>
</section>
<div class="backing-image" in:fade={{ duration: 1000 }} out:fly={{ x: 200, duration: 500 }}>
	<Image src="images/tommy-bickerdike.jpg" alt="Tommy Bickerdike" width="600" sizes="(max-width: 600px) 80vw, 500px" threshold="0.8"/>
</div>

<style>
	h1 {
		font-weight: inherit;
		position: relative;
		display: block;
		font-size: 5.5rem;
		padding-top: 12vh;
		line-height: 1.1;
		font-weight: 700;
		max-width: 66vw;
		margin: 0 0 1rem;
	}

	p {
		font-size: 1.5rem;
		width: 40ch;
		max-width: 100%;
	}

	@media (max-width: 700px) {
		h1 {
			font-size: 3.5rem;
		}
	}
</style>