<script lang="ts">
	import { goto } from '$app/navigation';
	import { page } from '$app/stores';
	import '../app.css';
	import { fade } from 'svelte/transition';
	import BackToTopButton from '$lib/components/BackToTopButton.svelte';

	let { children } = $props();
	const routes: string[] = ['Home', 'About', 'Contact'];

	let selectedRoute: string = $state('Home');

	$effect.pre(() => {
		const path = $page.url.pathname;
		if (path === '/') {
			selectedRoute = 'Home';
		} else {
			selectedRoute = path.substring(1).charAt(0).toUpperCase() + path.substring(2);
		}
	});

	function onRouteChange() {
		if (selectedRoute === 'Home') {
			goto('/');
		} else {
			goto(`/${selectedRoute.toLowerCase()}`);
		}
	}

	$effect(() => {
		const path = $page.url.pathname;
		if (path === '/') {
			selectedRoute = 'Home';
		} else {
			selectedRoute = path.substring(1).charAt(0).toUpperCase() + path.substring(2);
		}
	});
</script>

<div class="fixed top-0 z-20 m-2">
	<select
		bind:value={selectedRoute}
		onchange={onRouteChange}
		class="border-grey-600 block w-full border bg-black px-2 py-1 text-gray-200 shadow-sm transition-all focus:scale-105 focus:border-transparent focus:px-3 focus:py-2 focus:outline-none focus:ring-1 focus:ring-white"
	>
		{#each routes as route}
			<option value={route}>{route}</option>
		{/each}
	</select>
</div>

<main class="bg-black">
	{#key $page.url.pathname}
		<div in:fade={{ duration: 300 }}>
			{@render children()}
		</div>
	{/key}
	<BackToTopButton />
</main>
