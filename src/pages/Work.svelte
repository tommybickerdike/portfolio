<script>
  import Image from "svelte-image";
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
      <a href="https://www.musicglue.com/ac-dc/">
        AC/DC
        <div class="image">
          <div class="image-process">
            <Image src="images/ac-dc.jpg" alt="AC/DC Website" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </div>
      </a><br>
      <a href="https://www.entershikari.com">
        Enter Shikari
        <div class="image">
          <div class="image-process">
            <Image src="images/enter-shikari.jpg" alt="Enter Shikari Website" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </div>
      </a><br>
      <a href="https://merch.georgeezra.com">
        George Ezra
        <div class="image">
          <div class="image-process">
            <Image src="images/george-ezra.jpg" alt="George Ezra Website" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </div>
      </a><br>
      <a href="https://www.jacksavoretti.com">
        Jack Savoretti
        <div class="image">
          <div class="image-process">
            <Image src="images/jack-savoretti.jpg" alt="Jack Savoretti Website" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </div>
      </a><br>
      <a href="https://store.ledzeppelin.com">
        Led Zeppelin
        <div class="image">
          <div class="image-process">
            <Image src="images/led-zeppelin.jpg" alt="Led Zeppelin Website" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </div>
      </a><br>
      <a href="https://www.motorhead79.com">
        Motörhead
        <div class="image">
          <div class="image-process">
            <Image src="images/motorhead.jpg" alt="Motörhead Website" width="1500" height="1500" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </div>
      </a>
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
		position: fixed;
    pointer-events: none;
    transform: translate3d(-100%, 0, 1px);
		top: 0;
    opacity: 0;
    padding-top: 2rem;
		right: 0;
		height: 100vh;
		width: 600px;
		max-width: 80%;
		z-index: -1;
		background: #262C57;
    transition: .3s opacity, .5s transform;
	}

	.image-process {
		mix-blend-mode: multiply;
    opacity: .5;
	}

  a:hover .image {
    opacity: 1;
    transform: translate3d(0, 0, 1px);
  }
</style>