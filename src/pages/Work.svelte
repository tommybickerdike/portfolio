<script>
  import { fly } from "svelte/transition";
</script>

<svelte:head>
  <title>Tommy Bickerdike - Work</title>
</svelte:head>

<section in:fly={{ y: 50, duration: 500 }} out:fly={{ y: 50, duration: 500 }}>
  <div>
    <h2>Music Ecommerce</h2>
    <p>Artist websites designed & built on the Music Glue platform.</p>
    <p>
      <a href="https://www.musicglue.com/ac-dc/">AC/DC</a><br>
      <a href="https://www.entershikari.com">Enter Shikari</a><br>
      <a href="https://merch.georgeezra.com">George Ezra</a><br>
      <a href="https://www.jacksavoretti.com">Jack Savoretti</a><br>
      <a href="https://store.ledzeppelin.com">Led Zeppelin</a><br>
      <a href="https://www.motorhead79.com">Motörhead</a>
    </p>
  </div>
  <div>
    <h2>Branding</h2>
    <p>Brand logo, supporting styles and website UI. Developed in 2019.</p>
    <p>
      <a href="https://www.musicglue.com/">Visit Music Glue</a>
    </p>
  </div>
  <div>
    <h2>Advocacy</h2>
    <p>Design work for advocacy and social causes.</p>
    <p>
      <a href="https://extinctionrebellion.uk/">Extinction Rebelion WordPress website development.</a><br>
      <a href="http://menengage.org/wp-content/uploads/2019/11/Transforming-Masculinities.pdf">Men Engage Alliance Anual Report Design & Layout.</a>
    </p>
  </div>
</section>


<style>
  h2 {
    font-size: 2rem;
    margin: 0 0 1rem;
    padding: 0;
  }
  p {
    font-size: 1.5rem;
  }

  a {
    font-weight: bold;
    font-size: 1.25rem;
  }

  div {
    margin: 2rem 0 4rem;
  }
</style>