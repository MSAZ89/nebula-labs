<script lang="ts">
	import { onMount } from 'svelte';

	let showButton = $state(false);

	// Show button when user scrolls down 200px
	onMount(() => {
		const handleScroll = () => {
			showButton = window.scrollY > 200;
		};

		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<a
	aria-label="back-to-top-button"
	href="#top"
	class={`fixed bottom-8 right-8 flex h-12 w-12 items-center justify-center rounded-full border border-white/20 bg-black/80 text-white shadow-lg backdrop-blur-sm transition-all duration-300 hover:bg-white hover:text-black ${
		showButton ? 'translate-y-0 opacity-100' : 'translate-y-16 opacity-0'
	}`}
	on:click|preventDefault={(e) => {
		window.scrollTo({ top: 0, behavior: 'smooth' });
	}}
>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		class="h-6 w-6"
		fill="none"
		viewBox="0 0 24 24"
		stroke="currentColor"
	>
		<path
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-width="2"
			d="M5 10l7-7m0 0l7 7m-7-7v18"
		/>
	</svg>
</a>
