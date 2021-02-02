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
			<Link to="work">Work</Link>
		</nav>
	</header>
	<main>
		<Route path=""><Intro /></Route>
		<Route path="work" component="{Work}" /> 
	</main>
	<footer>
		Hello
	</footer>
</Router>
