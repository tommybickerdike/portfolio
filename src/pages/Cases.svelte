<script>
  import Image from "svelte-image";
  import { Router, Link, Route } from "svelte-routing";
  let url = "";
</script>

<Router url="{url}">
  <Route path="ecommerce-sites">
    <section>
      <h1>Music Ecommerce Websites</h1>
      <p>Artist websites designed & built on the Music Glue platform.</p>
      <p>
        <a target="_blank" href="https://www.musicglue.com/ac-dc/">
          AC/DC
          <div class="backing-image">
            <Image src="ac-dc.jpg" alt="AC/DC Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </a><br>
        <a target="_blank" href="https://www.entershikari.com">
          Enter Shikari
          <div class="backing-image">
            <Image src="enter-shikari.jpg" alt="Enter Shikari Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </a><br>
        <a target="_blank" href="https://merch.georgeezra.com">
          George Ezra
          <div class="backing-image">
            <Image src="george-ezra.jpg" alt="George Ezra Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </a><br>
        <a target="_blank" href="https://www.jacksavoretti.com">
          Jack Savoretti
          <div class="backing-image">
            <Image src="jack-savoretti.jpg" alt="Jack Savoretti Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </a><br>
        <a target="_blank" href="https://store.ledzeppelin.com">
          Led Zeppelin
          <div class="backing-image">
            <Image src="led-zeppelin.jpg" alt="Led Zeppelin Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
        </a><br>
        <a target="_blank" href="https://www.motorhead79.com">
          Motörhead
          <div class="backing-image">
            <Image src="motorhead.jpg" alt="Motörhead Website" width="600" sizes="(max-width: 600px) 80vw, 600px" threshold="0.8"/>
          </div>
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
  a {
    font-weight: bold;
    font-size: 1.25rem;
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