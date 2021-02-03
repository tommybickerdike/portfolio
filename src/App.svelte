<script>
  import { Router, Route, Link } from "svelte-routing";
  import Intro from "./pages/Intro.svelte";
  import Work from "./pages/Work.svelte";
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
		<Route path="/work" component="{Work}" /> 
	</main>
	<footer>
		Built with Svelte <a href="https://github.com/tommybickerdike/portfolio" target="_blank" rel="noopener">view source</a>.
	</footer>
</Router>