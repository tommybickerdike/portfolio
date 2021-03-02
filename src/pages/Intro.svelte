<svelte:head>
  <title>Tommy Bickerdike</title>
</svelte:head>

<script>
	import Image from "svelte-image";
	import { fly, fade } from "svelte/transition";
	import { Link } from "svelte-routing";
</script>

<section in:fly={{ x: 300, duration: 1000 }} out:fly={{ x: -300, duration: 500 }}>
	<h1>Tommy Bickerdike</h1>
	<p>A senior UX designer and front end developer working at Music Glue to create beautiful e-commerce stores.</p>
	<Link to="/work" rel="prefetch">See Work →</Link>
</section>
<div class="backing-image" in:fade={{ duration: 1000 }} out:fly={{ x: -300, duration: 500 }}>
	<Image src="images/tommy-bickerdike.jpg" alt="Tommy Bickerdike" width="600" sizes="(max-width: 600px) 80vw, 500px" threshold="0.8"/>
</div>

<style>
	h1 {
		font-weight: inherit;
		position: relative;
		display: block;
		font-size: 4rem;
		padding-top: 10vh;
		line-height: 1.1;
		font-weight: 700;
		max-width: 66vw;
		margin: 0 0 1rem;
	}

	p {
		width: 40ch;
		max-width: 100%;
	}

	@media (max-width: 700px) {
		h1 {
			padding-top: 15vh;
			font-size: 3rem;
		}
	}
</style>