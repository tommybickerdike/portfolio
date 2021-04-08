<svelte:head>
  <title>Tommy Bickerdike - Work</title>
</svelte:head>

<script>
  
  import Card from '../fragments/Card.svelte';
  import { fade } from "svelte/transition";
  import { link } from "svelte-routing";
</script>

<section in:fade={{ duration: 600 }}>
  <dl>
    <Card href={"/case-studies/ecommerce-sites"} image={"/images/venndr.jpg"}>
      <span slot="title">Platform UI Design</span> 
      <span slot="description">UI design and development for Music Glue.</span>
    </Card>
    
    <Card href={"/case-studies/second"} image={"/images/music-glue.jpg"}>
      <span slot="title">Platform UI Design</span> 
      <span slot="description">UI design and development for Music Glue.</span>
    </Card>
  </dl>
</section>


<style>
  dl { 
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
  }

  @media(max-width: 650px) {
    dl {
      grid-template-columns: repeat(1, 1fr);
    }
  }
</style>