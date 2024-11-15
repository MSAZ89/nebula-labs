<script lang="ts">
	export let text: string = 'Button';
	export let href: string = '/';
</script>

<a
	{href}
	title={text}
	class="mt-4 rounded-full border-2 border-black bg-transparent px-8 py-3 text-lg text-black transition duration-300 hover:bg-black hover:text-white"
	>{text}
</a>
