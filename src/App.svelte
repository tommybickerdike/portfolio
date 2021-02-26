<script>
  import { Router, Route, Link } from "svelte-routing";
  import Intro from "./pages/Intro.svelte";
  import Work from "./pages/Work.svelte";
	import Cases from "./pages/Cases.svelte";
  export let url = "";
</script>

<Router url="{url}">
	<header>
		<nav>
			<Link to="/">Intro</Link>
			<Link to="/work" rel="prefetch">Work</Link>
		</nav>
	</header>
	<main>
		<Route path=""><Intro /></Route>
		<Route path="work" component="{Work}" />
		<Route path="case-studies/*" component="{Cases}" />
	</main>
	<footer>
		Built by Tommy using Svelte <a href="https://github.com/tommybickerdike/portfolio" target="_blank" rel="noopener">view source</a>.
	</footer>
</Router>