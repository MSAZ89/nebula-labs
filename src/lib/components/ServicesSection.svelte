<script>
	const services = [
		{
			title: 'VR/AR Strategy Development',
			description:
				'Consulting for businesses looking to integrate immersive technology into their operations. We help you build the right strategy for your needs.'
		},
		{
			title: 'Custom VR/AR Solutions',
			description:
				'Tailored virtual environments and applications designed to meet your specific business needs, enhancing productivity and user experience.'
		},
		{
			title: 'Training & Support',
			description:
				'Expert training and ongoing support to ensure seamless adoption and effective use of VR/AR technology within your team or business.'
		},
		{
			title: 'Innovation Labs',
			description:
				'Stay ahead of the curve with regular updates and insights into emerging immersive technologies, helping your business explore new possibilities.'
		}
	];

	function scrollToWhy() {
		document.getElementById('why')?.scrollIntoView({ behavior: 'smooth' });
	}
</script>

<div
	id="services"
	class="relative flex min-h-screen flex-col items-center justify-center bg-fixed bg-center text-white"
	style="background-image: url('https://plus.unsplash.com/premium_photo-1663100703769-61c87c264693?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')"
>
	<!-- Overlay -->
	<div class="absolute inset-0 bg-black opacity-90" />

	<!-- Content -->
	<div
		class="relative z-10 flex flex-col items-center justify-center px-6 py-12 text-center lg:mx-64"
	>
		<h2
			class="mb-8 bg-gradient-to-r from-purple-400 to-purple-600 bg-clip-text text-4xl font-bold text-transparent"
		>
			Our Services
		</h2>
		<p class="mx-auto mb-12 max-w-3xl text-lg text-gray-300">
			We provide innovative solutions that empower businesses to stay ahead with cutting-edge VR/AR
			technologies. Explore our services and discover how we can help transform your operations.
		</p>

		<div class="grid grid-cols-1 gap-8 sm:grid-cols-2">
			{#each services as service}
				<div
					class="group relative overflow-hidden rounded-xl border border-purple-500/20 bg-black bg-opacity-50 p-8 backdrop-blur-sm transition-all duration-300 hover:scale-105 hover:transform hover:border-purple-500/40 hover:bg-opacity-70"
				>
					<!-- Gradient overlay -->
					<div
						class="absolute inset-0 bg-gradient-to-br from-purple-600/10 to-transparent opacity-0 transition-opacity duration-300 group-hover:opacity-100"
					/>

					<!-- Content -->
					<div class="relative z-10">
						<h3
							class="mb-4 text-2xl font-semibold text-white transition-colors duration-300 group-hover:text-purple-400"
						>
							{service.title}
						</h3>
						<p class="text-gray-300 transition-colors duration-300 group-hover:text-white">
							{service.description}
						</p>
					</div>
				</div>
			{/each}
		</div>

		<!-- Button -->
		<button
			on:click={scrollToWhy}
			class="mt-12 rounded-full bg-purple-600 px-8 py-3 font-semibold text-white transition-all duration-300 hover:bg-purple-700 hover:shadow-lg hover:shadow-purple-500/20"
		>
			Why Choose Us
		</button>
	</div>
</div>

<style>
	/* Add any component-specific styles here if needed */
</style>
