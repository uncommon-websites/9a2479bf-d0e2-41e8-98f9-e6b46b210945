<script lang="ts">
	import { ArrowUpRight } from 'lucide-svelte';
</script>

<header class="w-full px-4 md:px-8 py-6 flex items-center justify-between text-[14px] font-medium tracking-wide uppercase border-b border-transparent fixed top-0 left-0 z-50 bg-[#F4F4F2]/90 backdrop-blur-sm transition-all duration-300">
	<div class="flex-1">
		<a href="/" class="text-xl font-medium tracking-tighter">BOLD & VISIBLE</a>
	</div>

	<nav class="hidden md:flex items-center gap-12 text-gray-500">
		<a href="#method" class="hover:text-black transition-colors">Method</a>
		<a href="#programs" class="hover:text-black transition-colors">Programs</a>
		<a href="#about" class="hover:text-black transition-colors">About</a>
		<a href="#testimonials" class="hover:text-black transition-colors">Testimonials</a>
		<a href="#monologues" class="hover:text-black transition-colors">Monologues</a>
	</nav>

	<div class="flex-1 flex justify-end items-center gap-6 md:gap-8">
		<a href="#apply" class="flex items-center gap-1 hover:opacity-70 transition-opacity">
			<ArrowUpRight size={14} />
			APPLY
		</a>
		<a href="#contact" class="flex items-center gap-1 hover:opacity-70 transition-opacity">
			<ArrowUpRight size={14} />
			CONTACT
		</a>
	</div>
</header>
