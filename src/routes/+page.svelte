<script lang="ts">
	import "../app.css";
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

<div class="min-h-screen flex flex-col justify-between p-6 sm:p-8 md:p-12 lg:p-16 font-sans text-[#111] bg-white selection:bg-gray-200">
	<!-- Spacer for vertical centering alignment, but biased towards top/center -->
	<div class="flex-1 flex flex-col justify-center max-w-[900px]">
		
		<!-- Headline -->
		<h1 class="text-2xl sm:text-3xl md:text-[2rem] leading-[1.35] font-semibold tracking-tight mb-8 text-black">
			Thilo is <span class="inline-block bg-[#e5e5e5] px-2 py-0.5 font-semibold align-baseline">Uncommon</span> Founder, Partner and <span class="inline-block bg-[#e5e5e5] px-2 py-0.5 font-semibold align-baseline">Sequoia</span> Arc Advisor.
		</h1>

		<!-- Body Text -->
		<div class="text-lg sm:text-xl md:text-[1.35rem] leading-[1.6] text-[#999999] font-normal tracking-tight">
			He invested, advised or designed 
			{#each ["Mercor", "Delphi", "Squint", "Dash0", "CrewAI", "GradientLabs", "Build", "Fleet", "Medra", "nsave", "Ironbridge", "DiligenceSquared", "Lemni", "Morphic", "Compile", "Lapel", "Orbit", "Sensmore", "Nolla", "Luo", "Hero", "Popcorn", "Partykit", "Guided Energy", "Commerce Systems", "Claim", "Structify", "Snaptrude", "Superlinked", "Tilebox", "Amperecloud", "Equipme", "Documenso"] as company, i}
				<span class="inline-block bg-[#f0f0f0] text-[#666666] px-1.5 py-0.5 align-baseline">{company}</span>{#if i < 32}<span>, </span>{/if}
			{/each}
			and <span class="inline-block bg-[#f0f0f0] text-[#666666] px-1.5 py-0.5 align-baseline">Era</span>, founded <span class="inline-block bg-[#f0f0f0] text-[#666666] px-1.5 py-0.5 align-baseline">Home</span>, worked at <span class="inline-block bg-[#f0f0f0] text-[#666666] px-1.5 py-0.5 align-baseline">Airbnb</span> in 2011 and studied architecture – DM anytime on <span class="inline-block bg-[#f0f0f0] text-[#666666] px-1.5 py-0.5 align-baseline">X</span> or <span class="inline-block bg-[#f0f0f0] text-[#666666] px-1.5 py-0.5 align-baseline">LinkedIn</span>.
		</div>

		<!-- CTA -->
		<p class="mt-8 text-lg sm:text-xl md:text-[1.35rem] text-[#999999] font-normal tracking-tight">
			How can we work together?
		</p>
	</div>

	<!-- Footer -->
	<div class="flex justify-between items-end mt-12 w-full">
		<div class="text-[#cccccc] text-lg font-normal">Support with design</div>
		<button class="w-12 h-12 bg-[#e5e5e5] rounded-full flex items-center justify-center hover:bg-[#d5d5d5] transition-colors cursor-pointer" aria-label="Next">
			<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-[#888888]">
				<line x1="5" y1="12" x2="19" y2="12"></line>
				<polyline points="12 5 19 12 12 19"></polyline>
			</svg>
		</button>
	</div>
</div>

