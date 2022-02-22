<script>
  import Image from "svelte-image";
  import { fly } from "svelte/transition";
</script>

<svelte:head>
  <title>Tommy Bickerdike - Work</title>
</svelte:head>

<section in:fly={{ y: 50, duration: 500 }} out:fly={{ y: 50, duration: 500 }}>
  <div>
    <h2>UX Design</h2>
    <p>Music Glue platform UX design.</p>
    <a target="_blank" href="https://admin.musicglue.store/">
      Music Glue App
      <div class="image">
        <Image wrapperClass="image-wrap" src="images/venndr.jpg" alt="Music Glue App" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
      </div>
    </a>
  </div>
  <div>
    <h2>Ecommerce Websites</h2>
    <p>Artist websites designed & built on the Music Glue platform.</p>
    <p>
      <a target="_blank" href="https://www.musicglue.com/ac-dc/">
        AC/DC
        <div class="image">
          <Image wrapperClass="image-wrap" src="images/ac-dc.jpg" alt="AC/DC Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a><br>
      <a target="_blank" href="https://www.entershikari.com">
        Enter Shikari
        <div class="image">
          <Image wrapperClass="image-wrap" src="images/enter-shikari.jpg" alt="Enter Shikari Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a><br>
      <a target="_blank" href="https://merch.georgeezra.com">
        George Ezra
        <div class="image">
          <Image wrapperClass="image-wrap" src="images/george-ezra.jpg" alt="George Ezra Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a><br>
      <a target="_blank" href="https://www.jacksavoretti.com">
        Jack Savoretti
        <div class="image">
          <Image wrapperClass="image-wrap" src="images/jack-savoretti.jpg" alt="Jack Savoretti Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a><br>
      <a target="_blank" href="https://store.ledzeppelin.com">
        Led Zeppelin
        <div class="image">
          <Image wrapperClass="image-wrap" src="images/led-zeppelin.jpg" alt="Led Zeppelin Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a><br>
      <a target="_blank" href="https://www.motorhead79.com">
        Motörhead
        <div class="image">
          <Image wrapperClass="image-wrap" src="images/motorhead.jpg" alt="Motörhead Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a>
    </p>
  </div>
  <div>
    <h2>Branding</h2>
    <p>Brand logo, supporting styles and website UI. Developed in 2019.</p>
    <p>
      <a target="_blank" href="https://www.musicglue.com/">
        View Music Glue Website
        <div class="image">
          <Image wrapperClass="image-wrap" src="images/music-glue.jpg" alt="Music Glue Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a>
    </p>
  </div>
</section>


<style>
  section {
    z-index: 2;
  }
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
  .image {
    pointer-events: none;
	  transform: translate3d(-50%, 0, 1px);
	  opacity: 0;
    transition: .5s opacity, .3s transform;
  }

  a:hover .image {
    opacity: 1;
    transform: translate3d(0, 0, 1px);
  }
</style>
