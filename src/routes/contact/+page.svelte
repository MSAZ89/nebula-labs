<script>
	import PageInner from '$lib/components/pageInner.svelte';
</script>

<div class="min-h-screen bg-black">
	<div class="mx-auto max-w-4xl px-4 py-16">
		<PageInner title="Contact" heading="Get in Touch" />
		<p class="mb-8 text-center text-xl text-gray-300">
			Ready to explore the future of immersive technology? Let's connect.
		</p>

		<!-- Contact Form -->
		<div class="mt-12 rounded-2xl bg-gray-900/50 p-8 backdrop-blur-sm">
			<form class="space-y-6">
				<div class="grid gap-6 md:grid-cols-2">
					<!-- First Name -->
					<div>
						<label for="firstName" class="block text-sm font-medium text-gray-300">
							First Name
						</label>
						<input
							type="text"
							id="firstName"
							class="mt-1 w-full rounded-lg border border-gray-800 bg-gray-800/50 px-4 py-2.5 text-white placeholder-gray-400 focus:border-purple-500 focus:outline-none focus:ring-2 focus:ring-purple-500/20"
							placeholder="John"
						/>
					</div>

					<!-- Last Name -->
					<div>
						<label for="lastName" class="block text-sm font-medium text-gray-300">
							Last Name
						</label>
						<input
							type="text"
							id="lastName"
							class="mt-1 w-full rounded-lg border border-gray-800 bg-gray-800/50 px-4 py-2.5 text-white placeholder-gray-400 focus:border-purple-500 focus:outline-none focus:ring-2 focus:ring-purple-500/20"
							placeholder="Doe"
						/>
					</div>
				</div>

				<!-- Email -->
				<div>
					<label for="email" class="block text-sm font-medium text-gray-300"> Email Address </label>
					<input
						type="email"
						id="email"
						class="mt-1 w-full rounded-lg border border-gray-800 bg-gray-800/50 px-4 py-2.5 text-white placeholder-gray-400 focus:border-purple-500 focus:outline-none focus:ring-2 focus:ring-purple-500/20"
						placeholder="john@example.com"
					/>
				</div>

				<!-- Company -->
				<div>
					<label for="company" class="block text-sm font-medium text-gray-300">
						Company Name
					</label>
					<input
						type="text"
						id="company"
						class="mt-1 w-full rounded-lg border border-gray-800 bg-gray-800/50 px-4 py-2.5 text-white placeholder-gray-400 focus:border-purple-500 focus:outline-none focus:ring-2 focus:ring-purple-500/20"
						placeholder="Nebula Industries"
					/>
				</div>

				<!-- Project Type -->
				<div>
					<label for="projectType" class="block text-sm font-medium text-gray-300">
						Project Type
					</label>
					<select
						id="projectType"
						class="mt-1 w-full rounded-lg border border-gray-800 bg-gray-800/50 px-4 py-2.5 text-white placeholder-gray-400 focus:border-purple-500 focus:outline-none focus:ring-2 focus:ring-purple-500/20"
					>
						<option value="" disabled selected>Select a project type</option>
						<option value="vr">Virtual Reality Solution</option>
						<option value="ar">Augmented Reality Development</option>
						<option value="training">Immersive Training Platform</option>
						<option value="consulting">Technical Consulting</option>
						<option value="other">Other</option>
					</select>
				</div>

				<!-- Message -->
				<div>
					<label for="message" class="block text-sm font-medium text-gray-300">
						Project Details
					</label>
					<textarea
						id="message"
						rows="4"
						class="mt-1 w-full rounded-lg border border-gray-800 bg-gray-800/50 px-4 py-2.5 text-white placeholder-gray-400 focus:border-purple-500 focus:outline-none focus:ring-2 focus:ring-purple-500/20"
						placeholder="Tell us about your project..."
					></textarea>
				</div>

				<!-- Submit Button -->
				<div>
					<button
						type="submit"
						class="w-full rounded-lg bg-purple-600 px-6 py-3 text-base font-medium text-white transition-colors hover:bg-purple-700 focus:outline-none focus:ring-2 focus:ring-purple-500/20"
					>
						Send Message
					</button>
				</div>
			</form>
		</div>

		<!-- Contact Information -->
		<div class="mt-12 grid gap-8 text-center md:grid-cols-3">
			<div>
				<h3 class="text-lg font-semibold text-purple-400">Email</h3>
				<p class="mt-2 text-gray-300">contact@nebulalabs.tech</p>
			</div>
			<div>
				<h3 class="text-lg font-semibold text-purple-400">Phone</h3>
				<p class="mt-2 text-gray-300">+1 (555) 123-4567</p>
			</div>
			<div>
				<h3 class="text-lg font-semibold text-purple-400">Location</h3>
				<p class="mt-2 text-gray-300">San Francisco, CA</p>
			</div>
		</div>
	</div>
</div>

<style>
	select option {
		background-color: #1a1a1a;
		color: white;
	}
</style>
