<script lang="ts">
	import { Router, Link, Route } from 'svelte-routing';
import Index from './pages/Index.svelte';
import Machine from './pages/Machine.svelte';

	export let url = '';
</script>

<Router url="{url}">
	<Route path="run/:xurl" component="{Machine}" />
	<Route path="/"><Index /></Route>
</Router>
