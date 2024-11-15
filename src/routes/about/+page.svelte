<script>
	import PageInner from '$lib/components/pageInner.svelte';
	import BasicButtonBlack from '$lib/components/BasicButtonBlack.svelte';
	import BasicButton from '$lib/components/BasicButton.svelte';
</script>

<!-- Hero Section -->
<div
	style="background-image: url('https://plus.unsplash.com/premium_photo-1683134105531-42032fc66937?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')"
	class="relative flex h-screen flex-col items-center justify-center bg-cover bg-fixed bg-center text-white"
>
	<div class="absolute inset-0 bg-black/80"></div>
	<div class="relative z-10 px-4 text-center">
		<PageInner title="About" heading="About Nebula Labs" />
		<p class="mx-auto mb-8 max-w-3xl text-xl">
			At Nebula Labs, we specialize in developing cutting-edge VR/AR solutions that empower
			businesses to unlock new potential. Our team of experts pushes the boundaries of immersive
			technology to provide custom, future-ready solutions tailored to your unique needs.
		</p>
		<BasicButton href="#mission" text="Our Mission" />
	</div>
</div>

<!-- Our Mission Section -->
<section
	id="mission"
	class="relative flex h-screen items-center justify-center bg-gradient-to-b from-black to-gray-900 text-white"
>
	<div class="mx-auto max-w-4xl px-4 text-center">
		<h2 class="mb-6 text-4xl font-bold">Our Mission</h2>
		<p class="mb-8 text-xl leading-relaxed">
			Our mission at Nebula Labs is to revolutionize industries through immersive VR/AR experiences.
			By focusing on innovation, sustainability, and the future of digital interactions, we are
			committed to providing tailored solutions that increase operational efficiency, enhance user
			engagement, and transform the way businesses operate.
		</p>
		<BasicButton href="#what" text="What We Do" />
	</div>
</section>

<!-- What We Do Section -->
<section id="what" class="relative flex h-screen items-center justify-center bg-white text-black">
	<div class="mx-auto max-w-4xl px-4 text-center">
		<h2 class="mb-6 text-4xl font-bold">What We Do</h2>
		<p class="mb-8 text-xl leading-relaxed">
			At Nebula Labs, we offer a range of services designed to meet the needs of businesses in a
			variety of sectors. From custom VR/AR solutions to immersive training platforms and remote
			collaboration tools, we help companies integrate technology seamlessly to optimize their
			operations and enhance user experiences.
		</p>
		<BasicButtonBlack href="#team" text="Our Team" />
	</div>
</section>

<!-- Our Team Section -->
<section
	id="team"
	class="relative flex h-screen items-center justify-center bg-gradient-to-b from-gray-900 to-black text-white"
>
	<div class="mx-auto max-w-4xl px-4 text-center">
		<h2 class="mb-6 text-4xl font-bold">Our Team</h2>
		<p class="mb-8 text-xl leading-relaxed">
			The team at Nebula Labs is composed of passionate professionals with a deep understanding of
			immersive technologies. With diverse backgrounds in technology, design, and business strategy,
			we work together to deliver solutions that shape the future. Our expertise, creativity, and
			commitment to excellence ensure that we consistently push the limits of what's possible.
		</p>
		<BasicButton href="#values" text="Discover Our Values" />
	</div>
</section>

<!-- Our Values Section -->
<section id="values" class="relative flex h-screen items-center justify-center bg-white text-black">
	<div class="mx-auto max-w-4xl px-4 text-center">
		<h2 class="mb-6 text-4xl font-bold">Our Values</h2>
		<p class="mb-8 text-xl leading-relaxed">
			At Nebula Labs, we believe in integrity, innovation, and collaboration. We strive to build
			lasting relationships with our clients based on trust and mutual respect. Our values guide
			every decision, ensuring that we provide the highest quality solutions while fostering an
			environment that encourages creativity and continuous improvement.
		</p>
		<BasicButtonBlack href="#continue" text="Continue" />
	</div>
</section>

<!-- Call to Action Section -->
<section
	id="continue"
	class="relative flex h-screen items-center justify-center bg-gradient-to-b from-black to-gray-900 text-white"
>
	<div class="mx-auto max-w-4xl px-4 text-center">
		<h2 class="mb-6 text-4xl font-bold">Ready to Transform Your Business?</h2>
		<p class="mb-8 text-xl leading-relaxed">
			Partner with Nebula Labs and embrace the future of immersive technology. Whether you're
			looking to innovate your training programs, enhance client engagement, or explore new
			possibilities, we are here to help.
		</p>
		<BasicButton href="/contact" text="Contact Us Today" />
	</div>
</section>

<style>
	section {
		transition: background-color 0.5s ease;
	}
</style>
