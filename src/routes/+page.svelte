<script lang="ts">
	import "../app.css";
	import { onMount } from 'svelte';

	let revealed = $state(false);
	let currentTextIndex = $state(0);
	const footerTexts = ["Support with design", "Coinvest", "Advise"];

	onMount(() => {
		// Trigger reveal animation after mount
		setTimeout(() => {
			revealed = true;
		}, 100);

		// Rotate footer text every 2 seconds
		const interval = setInterval(() => {
			currentTextIndex = (currentTextIndex + 1) % footerTexts.length;
		}, 2000);

		return () => clearInterval(interval);
	});
</script>

<svelte:head>
	<title>KonZok - Design & Strategic Guidance for AI Startups</title>
	<meta name="description" content="Thilo Konzok connects founders with expert design and strategic guidance through hands-on product development partnerships. Uncommon Partner, Sequoia Arc Advisor, former Airbnb." />
	<meta property="og:title" content="KonZok - Design & Strategic Guidance for AI Startups" />
	<meta property="og:description" content="Thilo Konzok connects founders with expert design and strategic guidance through hands-on product development partnerships. Uncommon Partner, Sequoia Arc Advisor, former Airbnb." />
	<meta property="og:type" content="website" />
	<meta property="og:image" content="/og.png" />
	<meta name="twitter:card" content="summary_large_image" />
	<meta name="twitter:title" content="KonZok - Design & Strategic Guidance for AI Startups" />
	<meta name="twitter:description" content="Thilo Konzok connects founders with expert design and strategic guidance through hands-on product development partnerships. Uncommon Partner, Sequoia Arc Advisor, former Airbnb." />
	<meta name="twitter:image" content="/og.png" />
	<meta name="twitter:site" content="@thilokonzok" />
</svelte:head>

<div class="min-h-screen flex flex-col justify-between p-8 sm:p-12 md:p-16 lg:p-20 font-sans text-[#111] bg-[#f5f5f5] selection:bg-gray-300">
	<!-- Spacer for vertical centering alignment, but biased towards top/center -->
	<div class="flex-1 flex flex-col justify-start pt-12 sm:pt-16 md:pt-20 max-w-[1000px]">
		
		<!-- Headline -->
		<h1 class={[
			"text-2xl sm:text-3xl md:text-4xl lg:text-[2.5rem] leading-[1.3] font-bold tracking-tight mb-10 text-black transition-all duration-1000",
			revealed ? "blur-0 opacity-100" : "blur-sm opacity-0"
		]}>
			Thilo is Uncommon Founder, Partner and Sequoia Arc Advisor.
		</h1>

		<!-- Body Text -->
		<div class={[
			"text-lg sm:text-xl md:text-2xl lg:text-[1.5rem] leading-[1.65] text-[#999999] font-normal tracking-normal transition-all duration-1000 delay-200",
			revealed ? "blur-0 opacity-100" : "blur-sm opacity-0"
		]}>
			He invested, advised or designed Mercor, Delphi, Squint, Dash0, CrewAI, GradientLabs, Build, Fleet, Medra, nsave, Ironbridge, DiligenceSquared, Lemni, Morphic, Compile, Lapel, Orbit, Sensmore, Nolla, Luo, Hero, Popcorn, Partykit, Guided Energy, Commerce Systems, Claim, Structify, Snaptrude, Superlinked, Tilebox, Amperecloud, Equipme, Documenso and Era, founded Home, worked at Airbnb in 2011 and studied architecture – DM anytime on X or LinkedIn.
		</div>

		<!-- CTA -->
		<p class={[
			"mt-12 text-lg sm:text-xl md:text-2xl lg:text-[1.5rem] text-[#999999] font-normal tracking-normal transition-all duration-1000 delay-500",
			revealed ? "blur-0 opacity-100" : "blur-sm opacity-0"
		]}>
			How can we work together?
		</p>
	</div>

	<!-- Footer -->
	<div class="flex justify-between items-end mt-12 w-full">
		<div class="text-[#cccccc] text-base sm:text-lg font-normal transition-opacity duration-300">{footerTexts[currentTextIndex]}</div>
		<button class="w-14 h-14 bg-[#e0e0e0] rounded-full flex items-center justify-center hover:bg-[#d0d0d0] transition-colors cursor-pointer" aria-label="Next">
			<svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#999999]">
				<line x1="5" y1="12" x2="19" y2="12"></line>
				<polyline points="12 5 19 12 12 19"></polyline>
			</svg>
		</button>
	</div>
</div>

