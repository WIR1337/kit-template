<script lang="ts">
	import { onMount } from 'svelte';

	onMount(() => {
		// Type Assertation
		// Syntax
		let element = <HTMLDivElement>document.getElementById('qwe');
		// or
		let dick = document.getElementById('qwe') as HTMLDivElement;
	});

	interface Req {
		url: string;
		method: 'GET' | 'POST';
	}


	function handleRequest(url:string,method: 'GET'|'POST'){}

	const req = { url: 'https://example.com', method: 'GET' } as const;

	handleRequest(req.url, req.method);
</script>

<div id="qwe" />
<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
