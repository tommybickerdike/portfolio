<script>
  import { Router, Route, Link } from "svelte-routing";
  import Intro from "./pages/Intro.svelte";
  import Work from "./pages/Work.svelte";
  export let url = "";
</script>

<Router url="{url}">
	<nav>
		<Link to="/">Intro</Link>
		<Link to="work">Work</Link>
	</nav>
	<main>
		<Route path=""><Intro /></Route>
		<Route path="work" component="{Work}" /> 
	</main>
</Router>

<style>
	main {
		padding: 4rem;
		margin: 0 auto;
		min-height: 100vh;
		width: 100%;
		display: flex;
		position: relative;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
	}

	nav {
		position: fixed;
		top: 0;
	}

	@media (max-width: 65ch) {
		main {
			padding: 1rem;
			font-size: 13px;
		}
	}
</style>