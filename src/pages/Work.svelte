<svelte:head>
  <title>Tommy Bickerdike - Work</title>
</svelte:head>

<script>
  import Image from "svelte-image";
  import { fade } from "svelte/transition";
  import { Link } from "svelte-routing";
  import BackingImage from '../components/BackingImage.svelte';
</script>

<section in:fade={{ duration: 500 }}>
  <div>
    <h2>UX Design</h2>
    <p>Music Glue platform UX design.</p>
    <a target="_blank" href="https://admin.musicglue.store/">
      Music Glue App
      <BackingImage>
        <Image src="images/venndr.jpg" alt="Music Glue App" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
      </BackingImage>
      
    </a>
  </div>
  <div>
    <Link to="/case-studies/ecommerce-sites">Music Ecommerce Websites</Link>
  </div>
  <div>
    <h2>Branding</h2>
    <p>Brand logo, supporting styles and website UI. Developed in 2019.</p>
    <p>
      <a target="_blank" href="https://www.musicglue.com/">
        View Music Glue Website
        <div class="backing-image">
          <Image src="images/music-glue.jpg" alt="Music Glue Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a>
    </p>
  </div>
  <div>
    <h2>Advocacy</h2>
    <p>Design work for advocacy and social causes.</p>
    <p>
      <a target="_blank" href="https://extinctionrebellion.uk/">
        Extinction Rebelion WordPress website development.
        <div class="backing-image">
          <Image src="images/extinction-rebellion.jpg" alt="Extinction Rebellion Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </a><br>
      <a target="_blank" href="http://menengage.org/wp-content/uploads/2019/11/Transforming-Masculinities.pdf">
        Men Engage Alliance Annual Report Design & Layout.
        <div class="backing-image">
          <Image src="images/men-engage.jpg" alt="Men Engage Annual Report" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
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
    overflow: visible;
    position: relative;
  }

  div {
    margin: 2rem 0 4rem;
  }

</style>