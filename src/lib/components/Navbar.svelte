<script>
	let { isMenuOpen = false } = $props();
	let mobileMenuOpen = $state(false);
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-md border-b border-gray-200">
	<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
		<div class="flex justify-between items-center h-16">
			<!-- Logo -->
			<div class="flex items-center">
				<a href="/" class="flex items-center space-x-3">
					<img src="/logo.png" alt="Create MKT" class="h-8 w-auto" />
					<span class="text-xl font-bold text-gray-900">Create MKT</span>
				</a>
			</div>

			<!-- Desktop Navigation -->
			<div class="hidden md:block">
				<div class="ml-10 flex items-baseline space-x-8">
					<a href="#services" class="text-gray-700 hover:text-blue-600 px-3 py-2 text-sm font-medium transition-colors">Servicios</a>
					<a href="#portfolio" class="text-gray-700 hover:text-blue-600 px-3 py-2 text-sm font-medium transition-colors">Portafolio</a>
					<a href="#about" class="text-gray-700 hover:text-blue-600 px-3 py-2 text-sm font-medium transition-colors">Nosotros</a>
					<a href="#contact" class="text-gray-700 hover:text-blue-600 px-3 py-2 text-sm font-medium transition-colors">Contacto</a>
				</div>
			</div>

			<!-- CTA Button -->
			<div class="hidden md:block">
				<a href="#contact" class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-2 rounded-lg text-sm font-medium transition-colors">
					Comenzar
				</a>
			</div>

			<!-- Mobile menu button -->
			<div class="md:hidden">
				<button
					onclick={() => mobileMenuOpen = !mobileMenuOpen}
					class="inline-flex items-center justify-center p-2 rounded-md text-gray-700 hover:text-blue-600 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-blue-500"
					aria-expanded="false"
				>
					<span class="sr-only">Open main menu</span>
					{#if !mobileMenuOpen}
						<!-- Menu icon -->
						<svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
						</svg>
					{:else}
						<!-- Close icon -->
						<svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
						</svg>
					{/if}
				</button>
			</div>
		</div>
	</div>

	<!-- Mobile menu -->
	{#if mobileMenuOpen}
		<div class="md:hidden">
			<div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 bg-white border-t border-gray-200">
				<a href="#services" class="text-gray-700 hover:text-blue-600 block px-3 py-2 text-base font-medium">Servicios</a>
				<a href="#portfolio" class="text-gray-700 hover:text-blue-600 block px-3 py-2 text-base font-medium">Portafolio</a>
				<a href="#about" class="text-gray-700 hover:text-blue-600 block px-3 py-2 text-base font-medium">Nosotros</a>
				<a href="#contact" class="text-gray-700 hover:text-blue-600 block px-3 py-2 text-base font-medium">Contacto</a>
				<div class="pt-4 pb-2">
					<a href="#contact" class="bg-blue-600 hover:bg-blue-700 text-white block px-3 py-2 rounded-lg text-base font-medium text-center">
						Comenzar
					</a>
				</div>
			</div>
		</div>
	{/if}
</nav>