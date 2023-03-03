<script lang="ts">
	import { onMount } from "svelte";

	let a = 1 as number
	onMount(() => {
		// Type Assertation
		// Syntax
		let element = <HTMLDivElement>document.getElementById('qwe')
		// or
		let dick = document.getElementById('qwe') as HTMLDivElement

	})
</script>

<div id='qwe'></div>
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
