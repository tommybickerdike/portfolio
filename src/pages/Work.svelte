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
      <div class="card-img">
        <div class="img">
          <Image src="/images/venndr.jpg" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </div>
      <dt class="title">Platform UI Design</dt>
      <dd>UI design and development for Music Glue.</dd>
    </a>
    <a use:link href="/case-studies/ecommerce-sites">
      <div class="card-img">
        <div class="img">
          <Image src="/images/music-glue.jpg" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
        </div>
      </div>
      <dt class="title">Branding</dt>
      <dd>Brand logo, supporting styles and website UI. Developed in 2019.</dd>
    </a>
    <a use:link href="/case-studies/ecommerce-sites">
      <div class="card-img">
        <div class="img">
          <Image src="/images/george-ezra.jpg" width="600" sizes="(max-width: 600px) 80vw,  600px" threshold="0.8"/>
        </div>
      </div>
      <dt class="title">Ecommerce Website Development</dt>
      <dd>A wide range of bespoke e-commerce websites developed for music industry clients.</dd>
    </a>
  </dl>
</section>


<style>
  dl { 
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 2rem;
  }

  a {
    display: flex;
    flex-direction: column;
    background-color: var(--card-color);
    border-radius: .5rem;
    overflow: hidden;
    border: 1px solid var(--border-color);
    background: var(--card-color);
  }
  dt {
    font-size: 1.5rem;
    padding: 1rem 1rem 0 1rem;
    display: block;
  }
  dd {
    display: block;
    margin: 0;
    font-weight: normal;
    font-size: 1rem;
    padding: .5rem 1rem 1rem 1rem;
  }

  .card-img {
      width: 100%;
      height: 0;
      padding-bottom: 60%;
      overflow: hidden;
  }

  .img {
    transition: transform .2s;
  }

  @media(hover:hover) {
    a:hover {
      box-shadow: 0px 2px 4px var(--border-color);
    }
    a:hover .img {
      transform: scale(1.1);
    }
  }

</style>