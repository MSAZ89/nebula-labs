<script>
	import PageInner from '$lib/components/pageInner.svelte';
	import BasicButton from '$lib/components/BasicButton.svelte';
	import ServicesSection from '$lib/components/ServicesSection.svelte';
</script>

<div
	style="background-image: url('https://plus.unsplash.com/premium_photo-1663091706969-99390ffa1aad?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')"
	class="relative flex min-h-screen flex-col items-center justify-center bg-fixed bg-top text-white before:absolute before:inset-0 before:bg-black before:opacity-80"
>
	<div class="relative z-10 flex flex-col items-center justify-center">
		<PageInner title="Nebula Labs" heading="Nebula Labs" />
		<p class="mx-auto text-center text-xl">Empowering the Future of Virtual Innovation</p>
		<BasicButton href="#learn-more" text="Learn More" />
	</div>
</div>
<div
	id="learn-more"
	class="flex min-h-screen flex-col items-center justify-center bg-black text-white"
>
	<section
		id="About Nebula Labs"
		class="flex min-h-screen flex-col items-center justify-center bg-black text-white"
	>
		<div class="max-w-4xl border-b border-t border-white px-6 py-12">
			<h2 class="mb-6 text-4xl font-bold">About Nebula Labs</h2>
			<p class="text-lg leading-relaxed">
				At <strong>Nebula Labs</strong>, we're at the forefront of the virtual revolution. We
				specialize in delivering cutting-edge VR/AR solutions that transform how businesses engage
				with technology. From immersive training experiences to innovative remote collaboration
				tools, we help our clients unlock the full potential of immersive environments. With a
				passion for future-driven technology, our team is committed to pushing the boundaries of
				what's possible, shaping the future of digital interaction.
			</p>
			<p class="mt-4 text-lg leading-relaxed">
				Our mission is to empower businesses across industries—healthcare, education, real estate,
				and beyond—by providing custom, tailored virtual solutions that elevate user experience and
				efficiency. Whether you're looking to innovate your training programs, enhance client
				engagement, or explore new virtual possibilities, Nebula Labs is here to guide you into the
				next era of technology.
			</p>
		</div>
		<BasicButton href="#services" text="Services" />
	</section>
</div>
<ServicesSection />
<div
	id="why"
	class="mb-12 flex min-h-screen flex-col items-center justify-center bg-black text-white lg:mb-0"
>
	<section
		id="Why Choose Us"
		class="flex min-h-screen flex-col items-center justify-center bg-black text-white"
	>
		<div class="max-w-4xl border-b border-t border-white px-6 py-12">
			<h2 class="mb-6 text-4xl font-bold">Why Choose Us</h2>
			<p class="text-lg leading-relaxed">
				At <strong>Nebula Labs</strong>, we are pioneers in the field of immersive technology. We
				specialize in delivering innovative VR/AR solutions that redefine how businesses connect
				with their teams, clients, and customers. Our tailored virtual environments allow you to
				engage with technology in ways that were once unimaginable—transforming everything from
				training to collaboration, customer service, and beyond.
			</p>
			<p class="mt-4 text-lg leading-relaxed">
				Our mission is simple: to unlock the true potential of immersive technology for businesses
				across industries such as healthcare, education, real estate, and entertainment. We
				understand that each organization has unique needs, which is why we create custom solutions
				designed to improve operational efficiency, enhance learning experiences, and foster dynamic
				interactions. When you partner with Nebula Labs, you gain access to a team of experts
				passionate about delivering cutting-edge, future-ready technology solutions tailored to your
				success.
			</p>
		</div>
		<BasicButton href="#contact" text="Our Promise" />
	</section>
</div>
<div
	id="contact"
	style="background-image: url('https://plus.unsplash.com/premium_photo-1663054535424-8fa9da1e9724?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')"
	class="relative flex min-h-screen flex-col items-center justify-center bg-fixed bg-center text-white before:absolute before:inset-0 before:bg-black before:opacity-80"
>
	<div class="relative z-10 mb-12 flex flex-col items-center justify-center px-6 lg:mb-0">
		<h2 class="mb-8 mt-12 text-4xl font-semibold lg:mt-0">Our Promise</h2>
		<p class="mx-auto mb-12 max-w-3xl text-lg">
			At <strong>Nebula Labs</strong>, our promise is to empower businesses with innovative VR/AR
			solutions that transform industries. We are dedicated to pushing the boundaries of technology
			to deliver immersive experiences that drive efficiency, enhance engagement, and foster growth.
			Whether it's through custom virtual environments, interactive training modules, or advanced
			remote collaboration tools, our team is committed to bringing your business into the future.
		</p>
		<p class="mx-auto mb-12 max-w-3xl text-lg">
			We believe in the power of immersive technology to shape the way we work, learn, and interact.
			Our goal is to help you harness the full potential of VR/AR to solve real-world challenges,
			enhance decision-making, and improve user experiences. At Nebula Labs, we don’t just provide
			solutions—we partner with you to create a lasting impact on your business, guiding you every
			step of the way toward a smarter, more connected future.
		</p>

		<BasicButton href="/contact" text="Contact Nebula" />
	</div>
</div>
