<script>
  import { Router, Route, Link } from "svelte-routing";
  import Intro from "./pages/Intro.svelte";
  import Work from "./pages/Work.svelte";
  export let url = ""; //This property is necessary declare to avoid ignore the Router
</script>

<Router url="{url}">
	<nav>
		 <Link to="/">Intro</Link>
		 <Link to="work">Work</Link>
	 </nav>
	 <div>
		 <Route path="work" component="{Work}" /> 
		 <Route path="/"><Intro /></Route>
	 </div>
 </Router>