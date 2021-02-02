<script lang="ts">
	import Image from "svelte-image";
	import { fly } from "svelte/transition";
</script>

<svelte:head>
  <title>Tommy Bickerdike - Work</title>
</svelte:head>

<section in:fly={{ y: 50, duration: 500 }} out:fly={{ y: 50, duration: 500 }}>
	<h1>Machine &amp; Oil is the product design portfolio of <span>Tommy Bickerdike</span></h1>
</section>
<div class="image">
	<div class="image-process">
		<Image src="/tommy-bickerdike.png" alt="Tommy Bickerdike" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 500px"/>
	</div>
</div>


<style>
	section {
		z-index: 2;
	}
	h1 {
		font-weight: inherit;
		position: relative;
	}
	h1 span {
		display: block;
		font-size: 6rem;
		line-height: 1.1;
		font-weight: 700;
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
		h1 span {
			font-size: 4rem;
		}
	}
</style>