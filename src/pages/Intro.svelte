<script lang="ts">
	import Image from "svelte-image";
</script>



<div class="image">
	<div class="image-process">
		<Image src="/tommy-bickerdike.png" />
	</div>
</div>
<h1>Machine &amp; Oil is the product design portfolio of <span>Tommy Bickerdike</span></h1>


<style>
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