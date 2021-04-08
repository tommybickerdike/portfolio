<script>
  import { link } from "svelte-routing";
  import Image from "svelte-image";
  export let href;
  export let image;
</script>

<a use:link href={href}>
  <div class="card-img">
    <div class="img">
      <Image src={image} width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
    </div>
  </div>
  <dt><slot name="title"/></dt>
  <dd><slot name="description"/></dd>
</a>

<style>
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