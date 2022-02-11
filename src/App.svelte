<script>
	import { Router, Link, Route } from "svelte-routing";
	import Home from "./routes/Home.svelte";
	import Privacy from "./routes/Privacy.svelte";

	export let url = "";
</script>

<Router url="{url}">
	<nav>
		<Link to="/">Home</Link>
	</nav>
	<div>
		<Route path="privacy" component="{Privacy}" />
		<Route path="/"><Home /></Route>
	</div>
</Router>
