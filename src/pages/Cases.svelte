<script>
  import Image from "svelte-image";
  import { Router, Link, Route } from "svelte-routing";
  import BackingImage from '../components/BackingImage.svelte';
  export let url = "";
  export let basepath = "/";
</script>

<Router basepath={basepath} url="{url}">
  <Route path="ecommerce-sites">
    <section>
      <h1>Music Ecommerce Websites</h1>
      <p>Artist websites designed & built on the Music Glue platform.</p>
      <p>
        <a target="_blank" href="https://www.musicglue.com/ac-dc/">
          AC/DC
          <BackingImage>
            <Image src="/images/ac-dc.jpg" alt="AC/DC Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </BackingImage>
          
        </a><br>
        <a target="_blank" href="https://www.entershikari.com">
          Enter Shikari
          <BackingImage>
            <Image src="/images/enter-shikari.jpg" alt="Enter Shikari Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </BackingImage>
        </a><br>
        <a target="_blank" href="https://merch.georgeezra.com">
          George Ezra
          <BackingImage>
            <Image src="/images/george-ezra.jpg" alt="George Ezra Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </BackingImage>
        </a><br>
        <a target="_blank" href="https://www.jacksavoretti.com">
          Jack Savoretti
          <BackingImage>
            <Image src="/images/jack-savoretti.jpg" alt="Jack Savoretti Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </BackingImage>
        </a><br>
        <a target="_blank" href="https://store.ledzeppelin.com">
          Led Zeppelin
          <BackingImage>
            <Image src="/images/led-zeppelin.jpg" alt="Led Zeppelin Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </BackingImage>
        </a><br>
        <a target="_blank" href="https://www.motorhead79.com">
          Motörhead
          <BackingImage>
            <Image src="/images/motorhead.jpg" alt="Motörhead Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </BackingImage>
        </a>
      </p>
    </section>
    <Link to="second">Next →</Link>
  </Route>
  <Route path="second">
    <p>
      I did something awesome today. Lorem ipsum dolor sit amet, consectetur 
      adipisicing elit. Repudiandae enim quasi animi, vero deleniti dignissimos 
      sapiente perspiciatis. Veniam, repellendus, maiores.
    </p>
    <Link to="third">Next →</Link>
  </Route>
  <Link to="/work">← Work</Link>
</Router>


<style>
  
  
</style>