<svelte:head>
  <title>Tommy Bickerdike</title>
</svelte:head>

<script>
	import Image from "svelte-image";
	import BackingImage from '../components/BackingImage.svelte';
	import { fly } from "svelte/transition";
</script>

<section in:fly={{ y: 50, duration: 600 }} out:fly={{ y: 50, duration: 300 }}>
	<h1>Tommy Bickerdike</h1>
	<p>A senior UX designer and front end developer currently working in e-commerece at Music Glue.</p>
</section>
<BackingImage>
	<Image src="tommy-bickerdike.jpg" alt="Tommy Bickerdike" width="600" sizes="(max-width: 600px) 80vw, 500px" threshold="0.8"/>
</BackingImage>

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