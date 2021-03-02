<svelte:head>
  <title>Tommy Bickerdike - Work</title>
</svelte:head>

<script>
  import Image from "svelte-image";
  import { fade } from "svelte/transition";
  import { link } from "svelte-routing";
</script>

<section in:fade={{ duration: 600 }}>
  <dl>
    <a use:link href="/case-studies/ecommerce-sites">
      <dt class="title">Platform UI Design</dt>
      <dd>UI design and development for Music Glue.</dd>
      <div class="backing-image">
        <Image src="/images/venndr.jpg" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
      </div>
    </a>
    <a use:link href="/case-studies/ecommerce-sites">
      <dt class="title">Branding</dt>
      <dd>Brand logo, supporting styles and website UI. Developed in 2019.</dd>
      <div class="backing-image">
        <Image src="/images/music-glue.jpg" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
      </div>
    </a>
    <a use:link href="/case-studies/ecommerce-sites">
      <dt class="title">Ecommerce Website Development</dt>
      <dd>A wide range of bespoke e-commerce websites developed for music industry clients.</dd>
      <div class="backing-image">
        <Image src="/images/george-ezra.jpg" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
      </div>
    </a>
  </dl>
</section>


<style>
  section {
    z-index: 2;
  }
  dt {
    font-size: 1.5rem;
    margin: 0 0 1rem;
    padding: 0;
    display: block;
  }
  dd {
    display: block;
    margin: 0;
    font-weight: normal;
  }

  a {
    display: block;
    margin-bottom: 3rem;
  }
</style>