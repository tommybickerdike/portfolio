<script>
  import { fly } from "svelte/transition";
</script>

<svelte:head>
  <title>Tommy Bickerdike - Work</title>
</svelte:head>

<section in:fly={{ y: 50, duration: 500 }} out:fly={{ y: 50, duration: 500 }}>
  <h1>Check back soon</h1>
</section>
