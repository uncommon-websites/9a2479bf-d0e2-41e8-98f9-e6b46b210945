<script lang="ts">
	import Header from "$lib/components/Header.svelte";
	import { ArrowUpRight, ArrowRight } from 'lucide-svelte';

	const programs = [
		{ id: '01', name: 'THE PROGRAM', description: 'Group Coaching Journey' },
		{ id: '02', name: 'PRIVATE MENTORSHIP', description: 'One-on-One with Callie' },
		{ id: '03', name: 'CORPORATE PROGRAMS', description: 'Bespoke Group Coaching' },
		{ id: '04', name: 'BOLD & VISIBLE MONOLOGUES', description: 'Transformational Stage Experience' },
		{ id: '05', name: 'SOMATIC STORY METHOD™', description: 'Proprietary 7-Step Process' },
		{ id: '06', name: 'UNLEASH YOUR VOICE', description: 'Free Workshops' },
		{ id: '07', name: 'SPEAKING & EVENTS', description: 'Thought Leadership' }
	];

	const testimonials = [
		{ 
			name: 'KHERA', 
			role: 'Executive Coach, Entrepreneur', 
			quote: 'Total game changer for my life and business. I work with women at the highest levels of corporate France, and this work helped me relax, open my body, and become safe to get visible.',
			img: '/generated/image-confident-accomplished-woman-speaking-au-1765521630667-0.webp'
		},
		{ 
			name: 'KAREN', 
			role: 'PhD Psychologist', 
			quote: 'After 30 years in my field, I discovered new and exciting things about myself. This work is like nothing you have ever done before.',
			img: '/generated/image-woman-in-quiet-reflection-grounded-prese-1765521641109-4.webp'
		},
		{ 
			name: 'KIREI', 
			role: 'Business Owner, 5th Degree Black Belt', 
			quote: 'The depth and richness of this program gave me radical self-acceptance. I no longer shrink back. My business is expanding and flourishing.',
			img: '/generated/image-woman-speaking-confidently-to-camera-dir-1765521666620-14.webp'
		},
		{ 
			name: 'TECCA', 
			role: 'Storyteller, Leader Facilitator', 
			quote: 'This work changed my life. It created somatic safety around my challenges and blocks. I\'m more at ease with my authentic self and taking more risks with confidence.',
			img: '/generated/image-two-women-in-coaching-conversation-deep--1765521659259-11.webp'
		}
	];
</script>

<div class="min-h-screen bg-[#F4F4F2] text-[#1A1A1A] font-sans selection:bg-primary-600 selection:text-white overflow-x-hidden">
	<Header />

	<main>
		<!-- Hero Section -->
		<section class="pt-12 md:pt-20 pb-10 px-4 md:px-8">
			<div class="flex flex-col md:flex-row justify-between items-start mb-12 md:mb-24 relative">
				<div class="max-w-[200px] text-[10px] leading-relaxed uppercase tracking-wide font-medium mt-2">
					<p>Transforming accomplished women into visible leaders through somatic storytelling and nervous system regulation.</p>
				</div>
				<h1 class="text-[14vw] md:text-[9rem] lg:text-[11rem] leading-[0.8] font-thin tracking-tighter text-right mt-8 md:mt-0 uppercase">
					From <br />
					Invisible
				</h1>
			</div>

			<!-- Hero Images -->
			<div class="grid grid-cols-5 gap-2 md:gap-4 mb-8 h-[30vh] md:h-[50vh]">
				<div class="overflow-hidden h-full">
					<img src="/generated/image-confident-accomplished-woman-speaking-au-1765521630667-0.webp" alt="Confident woman speaking" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-woman-in-movement-somatic-practice-flowi-1765521633680-1.webp" alt="Somatic movement" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-professional-woman-storytelling-on-stage-1765521636193-2.webp" alt="Woman on stage" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-close-up-of-womans-hands-in-expressive-g-1765521638733-3.webp" alt="Expressive hands" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full">
					<img src="/generated/image-woman-in-quiet-reflection-grounded-prese-1765521641109-4.webp" alt="Grounded presence" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
			</div>

			<div class="flex flex-col md:flex-row justify-between items-start">
				<span class="text-[10px] uppercase tracking-wide font-medium mt-4 hidden md:block">Scroll</span>
				<h1 class="text-[14vw] md:text-[9rem] lg:text-[11rem] leading-[0.8] font-thin tracking-tighter text-right w-full uppercase">
					To <br />
					Bold & Visible
				</h1>
			</div>
		</section>

		<!-- Programs Section -->
		<section class="py-20 md:py-32" id="programs">
			<div class="flex justify-center mb-16 md:mb-24">
				<span class="text-[10px] font-bold uppercase tracking-widest">Programs & Offerings</span>
			</div>

			<div class="border-t border-gray-300">
				{#each programs as program}
					<div class="group border-b border-gray-300 py-6 md:py-10 px-4 md:px-8 flex items-center justify-between hover:bg-white transition-colors cursor-pointer">
						<span class="text-[10px] font-medium text-gray-500 w-8 md:w-12">/{program.id}</span>
						<div class="flex-1 text-center">
							<h2 class="text-3xl md:text-6xl lg:text-7xl font-thin tracking-tight group-hover:italic transition-all duration-300 uppercase">{program.name}</h2>
							<p class="text-[10px] uppercase tracking-wide font-medium text-gray-500 mt-2 opacity-0 group-hover:opacity-100 transition-opacity">{program.description}</p>
						</div>
						<div class="flex items-center gap-1 text-[10px] font-medium uppercase opacity-0 group-hover:opacity-100 transition-opacity translate-x-[-10px] group-hover:translate-x-0 duration-300">
							<ArrowUpRight size={12} />
							Learn More
						</div>
					</div>
				{/each}
			</div>
		</section>

		<!-- Testimonials Section -->
		<section class="py-20 px-4 md:px-8 bg-[#F4F4F2]" id="testimonials">
			<div class="flex flex-col md:flex-row justify-between items-start mb-16 md:mb-24">
				<h2 class="text-4xl md:text-6xl font-light tracking-tight mb-8 md:mb-0 uppercase">Transformations</h2>
				<div class="max-w-xs text-[10px] leading-relaxed uppercase tracking-wide font-medium text-right md:text-left">
					<p>Hear from accomplished women who have stepped into their visibility and transformed their lives and businesses.</p>
				</div>
			</div>

			<div class="grid grid-cols-1 md:grid-cols-2 gap-x-4 gap-y-12 md:gap-y-16">
				{#each testimonials as testimonial}
					<div class="group cursor-pointer">
						<div class="aspect-[3/4] overflow-hidden mb-4 bg-gray-200">
							<img src={testimonial.img} alt={testimonial.name} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
						</div>
						<h3 class="text-xs font-bold uppercase tracking-wide mb-1">{testimonial.name}</h3>
						<p class="text-[10px] text-gray-500 uppercase tracking-wide mb-3">{testimonial.role}</p>
						<p class="text-[10px] leading-relaxed font-medium mb-3">{testimonial.quote}</p>
					</div>
				{/each}
			</div>
		</section>

		<!-- Method & About Section -->
		<section class="py-20 px-4 md:px-8" id="method">
			<div class="flex flex-col lg:flex-row mb-16 gap-12 lg:gap-24">
				<div class="flex-1">
					<h2 class="text-4xl md:text-6xl font-light tracking-tight uppercase">The Method</h2>
				</div>
				<div class="flex-1">
					<h2 class="text-3xl md:text-5xl font-light tracking-tight mb-8 text-left uppercase leading-tight">Somatic Transformational<br/>Story Method™</h2>
					<div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-[10px] leading-relaxed uppercase tracking-wide font-medium">
						<p>Our proprietary seven-step embodied process—Awaken, Release, Source, Craft, Embody, Cross the Threshold, Integrate—combines somatic education, embodiment coaching, and performing arts practices to build a platform of somatic safety.</p>
						<p>We help accomplished female therapists, coaches, and entrepreneurs turn their personal story into visibility, authority, and thriving purpose-driven businesses. Through nervous system regulation and trauma-informed somatic movement, we address the fundamental lack of safety to speak up and be seen.</p>
					</div>
					<a href="#about" class="inline-flex items-center gap-1 text-[10px] font-medium uppercase mt-8 hover:opacity-60 transition-opacity">
						<ArrowUpRight size={10} />
						About Callie
					</a>
				</div>
			</div>

			<div class="flex flex-col md:flex-row gap-4 h-[50vh] md:h-[70vh]">
				<div class="w-full md:w-[60%] h-full bg-gray-200 overflow-hidden">
					<img src="/generated/image-small-group-of-women-in-circle-somatic-c-1765521646766-6.webp" alt="Group coaching session" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
				</div>
				<div class="w-full md:w-[40%] h-full flex flex-col gap-4">
					<div class="flex-1 bg-gray-200 overflow-hidden">
						<img src="/generated/image-woman-practicing-breathwork-eyes-closed--1765521649318-7.webp" alt="Breathwork practice" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
					</div>
					<div class="flex-1 flex gap-4">
						<div class="flex-1 bg-gray-200 overflow-hidden">
							<img src="/generated/image-woman-writing-in-journal-reflective-mome-1765521652090-8.webp" alt="Story crafting" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
						</div>
						<div class="flex-1 bg-gray-200 overflow-hidden">
							<img src="/generated/image-woman-standing-confidently-embodied-post-1765521654541-9.webp" alt="Embodied confidence" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- About Callie Section -->
		<section class="py-20 px-4 md:px-8 bg-[#F4F4F2]" id="about">
			<div class="flex flex-col lg:flex-row gap-12 lg:gap-24 items-center">
				<div class="w-full lg:w-1/3">
					<div class="aspect-[3/4] overflow-hidden bg-gray-200">
						<img src="/generated/image-mature-accomplished-woman-warm-confident-1765521644264-5.webp" alt="Callie B. Elwayns" class="w-full h-full object-cover" />
					</div>
				</div>
				<div class="flex-1">
					<h2 class="text-4xl md:text-6xl font-light tracking-tight mb-8 uppercase">Callie B. Elwayns</h2>
					<p class="text-xs uppercase tracking-wide font-medium text-gray-500 mb-8">Founder & Curator</p>
					<div class="space-y-6 text-[14px] leading-relaxed uppercase tracking-wide font-medium">
						<p>Callie survived homelessness as a youth, then led public companies for 20+ years. Her personal trauma journey gives her deep empathy for accomplished women hiding behind professional success, while her CEO experience proves she understands high-stakes leadership visibility.</p>
						<p>At age 20, her lungs collapsed for the first time—a result of genetics combined with survival trauma from her homeless years. She describes living in "chronic invisibility patterns" despite outward success, feeling isolated and unseen at a core level while appearing confident and accomplished.</p>
						<p>Through years of applied research as a trauma-informed somatic movement educator, Callie developed the Somatic Transformational Story Method™—a category-defining approach to embodied storytelling, presence, and leadership that helps women build a platform of somatic safety to be boldly visible.</p>
					</div>
				</div>
			</div>
		</section>

		<!-- CTA Section -->
		<section class="py-32 px-4 md:px-8 bg-[#1A1A1A] text-white text-center" id="apply">
			<span class="text-[10px] font-medium uppercase tracking-widest mb-6 block opacity-80">Your Mission Requires You</span>
			<h2 class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mb-8 uppercase">
				It's Time To <br />
				Get Visible
			</h2>
			<p class="text-[10px] uppercase tracking-wide font-medium mb-12 max-w-md mx-auto opacity-80">
				There has never been a more important moment when your voice and contributions have been needed on this planet.
			</p>
			<a href="#contact" class="inline-block bg-white text-[#1A1A1A] px-10 py-4 rounded-full text-[10px] font-bold uppercase tracking-widest hover:bg-primary-500 hover:text-white transition-colors">
				Apply Now
			</a>
		</section>

		<!-- Monologues Gallery -->
		<div class="grid grid-cols-2 md:grid-cols-5 h-[60vh]" id="monologues">
			<div class="overflow-hidden">
				<img src="/generated/image-woman-on-stage-sharing-story-authentic-e-1765521656853-10.webp" alt="Bold & Visible Monologues" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden">
				<img src="/generated/image-two-women-in-coaching-conversation-deep--1765521659259-11.webp" alt="Coaching connection" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden">
				<img src="/generated/image-woman-in-movement-practice-embodied-expr-1765521661757-12.webp" alt="Embodied movement" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden">
				<img src="/generated/image-group-of-accomplished-women-celebrating--1765521664252-13.webp" alt="Community celebration" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden hidden md:block">
				<img src="/generated/image-woman-speaking-confidently-to-camera-dir-1765521666620-14.webp" alt="Visible leadership" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
		</div>

		<!-- Footer Marquee -->
		<div class="overflow-hidden py-6 border-b border-gray-200">
			<div class="whitespace-nowrap animate-marquee flex">
				<span class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mx-4 uppercase">From invisible to bold & visible — Living life as art — From invisible to bold & visible — </span>
				<span class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mx-4 uppercase">From invisible to bold & visible — Living life as art — From invisible to bold & visible — </span>
			</div>
		</div>
	</main>

	<footer class="px-4 md:px-8 py-12 text-[14px] font-medium uppercase tracking-wide" id="contact">
		<div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-12 md:gap-8">
			<div class="flex flex-col gap-3">
				<a href="#method" class="hover:opacity-60">Method</a>
				<a href="#programs" class="hover:opacity-60">Programs</a>
				<a href="#about" class="hover:opacity-60">About</a>
				<a href="#testimonials" class="hover:opacity-60">Testimonials</a>
				<a href="#monologues" class="hover:opacity-60">Monologues</a>
			</div>

			<div class="text-left md:text-center">
				<p class="text-lg md:text-2xl font-normal tracking-tight mb-6">HELLO@BOLDANDVISIBLE.COM</p>
				<p class="text-xs tracking-widest mb-2">Institute for Feminine Somatic</p>
				<p class="text-xs tracking-widest">Integration and Wholeness</p>
			</div>

			<div class="flex flex-col gap-3 text-left md:text-right">
				<a href="#apply" class="hover:opacity-60">Apply Now</a>
				<a href="#privacy" class="hover:opacity-60">Privacy Policy</a>
				<a href="#terms" class="hover:opacity-60">Terms & Conditions</a>
			</div>
		</div>

		<div class="flex flex-col md:flex-row justify-between items-center mt-20 pt-8 border-t border-gray-200 text-[14px] text-gray-400 gap-4">
			<p>©BOLD & VISIBLE. ALL RIGHTS RESERVED</p>
			<div class="flex items-center gap-1">
				<span class="text-black text-lg font-bold tracking-tight">BOLD & VISIBLE</span>
			</div>
			<p>SOMATIC TRANSFORMATIONAL STORY METHOD™</p>
		</div>
	</footer>
</div>

<style>
	@keyframes marquee {
		0% { transform: translateX(0); }
		100% { transform: translateX(-50%); }
	}
	.animate-marquee {
		animation: marquee 30s linear infinite;
	}
</style>

