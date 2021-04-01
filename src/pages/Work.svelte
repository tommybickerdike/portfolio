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
      <div class="bg">
        <Image src="/images/venndr.jpg" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
      </div>
    </a>
    <a use:link href="/case-studies/ecommerce-sites">
      <dt class="title">Branding</dt>
      <dd>Brand logo, supporting styles and website UI. Developed in 2019.</dd>
      <div class="bg">
        <Image src="/images/music-glue.jpg" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
      </div>
    </a>
    <a use:link href="/case-studies/ecommerce-sites">
      <dt class="title">Ecommerce Website Development</dt>
      <dd>A wide range of bespoke e-commerce websites developed for music industry clients.</dd>
      <div class="bg">
        <Image src="/images/george-ezra.jpg" width="600" sizes="(max-width: 600px) 80vw,  600px" threshold="0.8"/>
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
    padding: 0;
    display: block;
    position: relative;
    z-index: 2;
  }
  dd {
    display: block;
    margin: 0;
    font-weight: normal;
    position: relative;
    z-index: 2;
  }
  dl { 
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
  }

  .bg {
      position: relative;
      width: 100%;
  }

  @media(hover:hover) {
    dl a { 
      position: relative;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      text-align: center;
      min-height: 15rem;
      padding: 1rem;
      align-items: center;
      justify-content: center;
    }
    .bg {
      position: absolute;
      width: 100%;
      z-index: -1;
      height: auto;
      top: 0;
      left: 0;
    }
  }
</style>