<script>
  import { fly, fade } from "svelte/transition";
</script>

<div class="backing-image" in:fade={{ duration: 2000 }} out:fly={{ x: 100, duration: 300 }}>
  <slot></slot>
</div>
