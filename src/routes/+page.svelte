<script>
	import Navbar from '$lib/components/Navbar.svelte';
</script>

<Navbar />

<main class="pt-16">
	<!-- Hero Section -->
	<section class="relative min-h-screen bg-gradient-to-br from-slate-900 via-purple-900 to-slate-900 overflow-hidden">
		<!-- Animated background elements -->
		<div class="absolute inset-0">
			<div class="absolute top-1/4 left-1/4 w-72 h-72 bg-purple-500/20 rounded-full blur-3xl animate-pulse"></div>
			<div class="absolute top-3/4 right-1/4 w-96 h-96 bg-blue-500/20 rounded-full blur-3xl animate-pulse delay-1000"></div>
			<div class="absolute top-1/2 left-1/2 w-80 h-80 bg-indigo-500/10 rounded-full blur-3xl animate-pulse delay-500"></div>
		</div>

		<!-- Grid pattern overlay -->
		<div class="absolute inset-0 opacity-20">
			<div class="absolute inset-0" style="background-image: radial-gradient(circle at 2px 2px, rgba(255,255,255,0.15) 1px, transparent 0); background-size: 50px 50px;"></div>
		</div>

		<div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 pt-20 pb-16">
			<div class="grid lg:grid-cols-2 gap-12 items-center min-h-[80vh]">
				
				<!-- Left Column - Content -->
				<div class="space-y-8">
					<!-- Badge -->
					<div class="inline-flex items-center px-4 py-2 bg-gradient-to-r from-purple-500/20 to-blue-500/20 rounded-full border border-white/20 backdrop-blur-sm">
						<div class="w-2 h-2 bg-green-400 rounded-full mr-2 animate-pulse"></div>
						<span class="text-sm text-white/90 font-medium">Disponibles para nuevos proyectos</span>
					</div>

					<!-- Main Headline -->
					<div class="space-y-4">
						<h1 class="text-5xl lg:text-7xl font-extrabold text-white leading-tight">
							Convertimos tu
							<span class="bg-gradient-to-r from-purple-400 to-blue-400 bg-clip-text text-transparent">
								visión
							</span>
							en marketing viral
						</h1>
						<p class="text-xl lg:text-2xl text-gray-300 leading-relaxed">
							Crecimiento explosivo, marcas inolvidables y campañas que convierten. 
							No solo hacemos marketing – creamos movimientos.
						</p>
					</div>

					<!-- Stats -->
					<div class="grid grid-cols-3 gap-8 py-8">
						<div class="text-center">
							<div class="text-3xl lg:text-4xl font-bold text-white mb-1">500%</div>
							<div class="text-sm text-gray-400 uppercase tracking-wide">Aumento ROI Promedio</div>
						</div>
						<div class="text-center">
							<div class="text-3xl lg:text-4xl font-bold text-white mb-1">50M+</div>
							<div class="text-sm text-gray-400 uppercase tracking-wide">Impresiones Generadas</div>
						</div>
						<div class="text-center">
							<div class="text-3xl lg:text-4xl font-bold text-white mb-1">200+</div>
							<div class="text-sm text-gray-400 uppercase tracking-wide">Marcas Transformadas</div>
						</div>
					</div>

					<!-- CTA Buttons -->
					<div class="flex flex-col sm:flex-row gap-4">
						<a href="#contact" class="group relative inline-flex items-center px-8 py-4 bg-gradient-to-r from-purple-600 to-blue-600 text-white font-semibold rounded-xl hover:from-purple-700 hover:to-blue-700 transition-all duration-300 shadow-2xl shadow-purple-500/25 hover:shadow-purple-500/40 transform hover:-translate-y-1">
							<span>Inicia Tu Transformación</span>
							<svg class="w-5 h-5 ml-2 group-hover:translate-x-1 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7l5 5m0 0l-5 5m5-5H6"></path>
							</svg>
						</a>
						<a href="#portfolio" class="inline-flex items-center px-8 py-4 border-2 border-white/20 text-white font-semibold rounded-xl hover:bg-white/10 hover:border-white/40 transition-all duration-300 backdrop-blur-sm">
							Ver Nuestro Trabajo
						</a>
					</div>

					<!-- Social Proof -->
					<div class="pt-8">
						<p class="text-sm text-gray-400 mb-4">Confianza de líderes de la industria:</p>
						<div class="flex items-center space-x-6 opacity-60">
							<div class="text-white font-semibold">NIKE</div>
							<div class="text-white font-semibold">APPLE</div>
							<div class="text-white font-semibold">TESLA</div>
							<div class="text-white font-semibold">AIRBNB</div>
						</div>
					</div>
				</div>

				<!-- Right Column - Visual -->
				<div class="relative lg:pl-8">
					<!-- Main visual container -->
					<div class="relative">
						<!-- Floating cards/elements -->
						<div class="absolute inset-0">
							<!-- Chart/Graph element -->
							<div class="absolute top-8 right-8 bg-white/10 backdrop-blur-md rounded-2xl p-6 border border-white/20 animate-float">
								<div class="flex items-center justify-between mb-4">
									<span class="text-white text-sm font-medium">Crecimiento ROI</span>
									<span class="text-green-400 text-xs">+127%</span>
								</div>
								<div class="h-20 flex items-end justify-between space-x-2">
									<div class="bg-gradient-to-t from-purple-500 to-purple-400 w-3 h-8 rounded-full"></div>
									<div class="bg-gradient-to-t from-purple-500 to-purple-400 w-3 h-12 rounded-full"></div>
									<div class="bg-gradient-to-t from-purple-500 to-purple-400 w-3 h-16 rounded-full"></div>
									<div class="bg-gradient-to-t from-purple-500 to-purple-400 w-3 h-20 rounded-full"></div>
								</div>
							</div>

							<!-- Notification element -->
							<div class="absolute top-32 left-4 bg-white/10 backdrop-blur-md rounded-xl p-4 border border-white/20 animate-float delay-300">
								<div class="flex items-center space-x-3">
									<div class="w-3 h-3 bg-green-400 rounded-full animate-pulse"></div>
									<span class="text-white text-sm">Campaña Activa</span>
								</div>
								<div class="text-gray-300 text-xs mt-1">+2.4K conversiones hoy</div>
							</div>

							<!-- Metrics card -->
							<div class="absolute bottom-16 left-8 bg-white/10 backdrop-blur-md rounded-xl p-4 border border-white/20 animate-float delay-700">
								<div class="text-white text-lg font-bold">1.2M</div>
								<div class="text-gray-300 text-xs">Alcance Mensual</div>
							</div>

							<!-- Social engagement -->
							<div class="absolute bottom-8 right-4 bg-white/10 backdrop-blur-md rounded-xl p-4 border border-white/20 animate-float delay-1000">
								<div class="flex items-center space-x-2 mb-2">
									<div class="w-6 h-6 bg-gradient-to-r from-pink-500 to-red-500 rounded-full flex items-center justify-center">
										<span class="text-white text-xs">❤️</span>
									</div>
									<span class="text-white text-sm font-medium">Post Viral</span>
								</div>
								<div class="text-gray-300 text-xs">850K interacciones</div>
							</div>
						</div>

						<!-- Central glow effect -->
						<div class="relative w-96 h-96 mx-auto">
							<div class="absolute inset-0 bg-gradient-to-r from-purple-500/30 to-blue-500/30 rounded-full blur-3xl"></div>
							<div class="absolute inset-8 bg-gradient-to-r from-purple-600/40 to-blue-600/40 rounded-full blur-2xl"></div>
							<div class="absolute inset-16 bg-gradient-to-r from-purple-700/50 to-blue-700/50 rounded-full blur-xl"></div>
						</div>
					</div>
				</div>

			</div>
		</div>

		<!-- Bottom wave -->
		<div class="absolute bottom-0 left-0 right-0">
			<svg viewBox="0 0 1440 120" class="w-full h-20 fill-white">
				<path d="M0,64L48,69.3C96,75,192,85,288,85.3C384,85,480,75,576,64C672,53,768,43,864,48C960,53,1056,75,1152,80C1248,85,1344,75,1392,69.3L1440,64L1440,120L1392,120C1344,120,1248,120,1152,120C1056,120,960,120,864,120C768,120,672,120,576,120C480,120,384,120,288,120C192,120,96,120,48,120L0,120Z"></path>
			</svg>
		</div>
	</section>
</main>

<style>
	@keyframes float {
		0%, 100% { transform: translateY(0px); }
		50% { transform: translateY(-10px); }
	}
	
	.animate-float {
		animation: float 3s ease-in-out infinite;
	}
	
	.delay-300 {
		animation-delay: 0.3s;
	}
	
	.delay-700 {
		animation-delay: 0.7s;
	}
	
	.delay-1000 {
		animation-delay: 1s;
	}
</style>
