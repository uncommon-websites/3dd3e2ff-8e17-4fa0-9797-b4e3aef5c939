<script lang="ts">
	import "../app.css";
</script>

<svelte:head>
	<title>KonZok — Design and Strategy for AI Founders</title>
	<meta name="description" content="Thilo Konzok brings design thinking and product expertise to early-stage AI startups. Partner at Uncommon, Sequoia Arc Advisor, former Airbnb. 40+ investments including Mercor, CrewAI, Delphi." />
	<meta property="og:title" content="KonZok — Design and Strategy for AI Founders" />
	<meta property="og:description" content="Thilo Konzok brings design thinking and product expertise to early-stage AI startups. Partner at Uncommon, Sequoia Arc Advisor, former Airbnb. 40+ investments including Mercor, CrewAI, Delphi." />
	<meta property="og:type" content="website" />
	<meta property="og:image" content="/og.png" />
	<meta name="twitter:card" content="summary_large_image" />
	<meta name="twitter:title" content="KonZok — Design and Strategy for AI Founders" />
	<meta name="twitter:description" content="Thilo Konzok brings design thinking and product expertise to early-stage AI startups. Partner at Uncommon, Sequoia Arc Advisor, former Airbnb. 40+ investments including Mercor, CrewAI, Delphi." />
	<meta name="twitter:image" content="/og.png" />
	<meta name="twitter:site" content="@thilokonzok" />
</svelte:head>

<div class="min-h-screen flex flex-col p-6 sm:p-8 md:p-12 lg:p-16 font-sans text-[#111] bg-white selection:bg-gray-200">
	
	<!-- Header -->
	<header class="mb-20 md:mb-32">
		<div class="text-sm tracking-wide text-[#999999] font-medium uppercase">KonZok</div>
	</header>

	<!-- Main Content -->
	<main class="flex-1 max-w-[960px]">
		
		<!-- Hero -->
		<section class="mb-20 md:mb-28">
			<h1 class="text-[1.75rem] sm:text-2xl md:text-[2.25rem] leading-[1.3] font-semibold tracking-tight mb-6 text-black max-w-[720px]">
				Design and strategy for founders building what's next.
			</h1>
			<p class="text-lg sm:text-xl md:text-[1.35rem] leading-[1.55] text-[#888888] font-normal tracking-tight max-w-[640px]">
				Thilo Konzok brings architecture-trained design thinking, early <span class="text-[#555555]">Airbnb</span> product instincts, and pattern recognition from 40+ investments to help AI founders go from idea to launch.
			</p>
		</section>

		<!-- Background -->
		<section class="mb-16 md:mb-24">
			<h2 class="text-xs font-medium uppercase tracking-widest text-[#bbbbbb] mb-6">Background</h2>
			<div class="space-y-3 text-[1.05rem] sm:text-[1.1rem] leading-[1.6] text-[#666666]">
				<p>
					<span class="text-[#333333] font-medium">Uncommon</span> — Founder & Partner, investing in early-stage companies
				</p>
				<p>
					<span class="text-[#333333] font-medium">Sequoia Arc</span> — Advisor to accelerator cohorts
				</p>
				<p>
					<span class="text-[#333333] font-medium">Airbnb</span> — Product team during hypergrowth, 2011
				</p>
				<p>
					<span class="text-[#333333] font-medium">Architecture</span> — Trained in spatial thinking and systems design
				</p>
			</div>
		</section>

		<!-- Portfolio -->
		<section class="mb-16 md:mb-24">
			<h2 class="text-xs font-medium uppercase tracking-widest text-[#bbbbbb] mb-6">Portfolio</h2>
			
			<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-x-8 gap-y-6">
				<!-- AI & Infrastructure -->
				<div>
					<h3 class="text-[0.7rem] font-medium uppercase tracking-wider text-[#aaaaaa] mb-3">AI & Infrastructure</h3>
					<div class="flex flex-wrap gap-2">
						{#each ['Mercor', 'CrewAI', 'Delphi', 'GradientLabs', 'Structify', 'Superlinked'] as company}
							<span class="inline-block bg-[#f5f5f5] text-[#555555] px-2 py-1 text-sm">{company}</span>
						{/each}
					</div>
				</div>

				<!-- Developer Tools -->
				<div>
					<h3 class="text-[0.7rem] font-medium uppercase tracking-wider text-[#aaaaaa] mb-3">Developer Tools</h3>
					<div class="flex flex-wrap gap-2">
						{#each ['Dash0', 'Squint', 'Compile', 'Orbit', 'Partykit'] as company}
							<span class="inline-block bg-[#f5f5f5] text-[#555555] px-2 py-1 text-sm">{company}</span>
						{/each}
					</div>
				</div>

				<!-- Fintech -->
				<div>
					<h3 class="text-[0.7rem] font-medium uppercase tracking-wider text-[#aaaaaa] mb-3">Fintech</h3>
					<div class="flex flex-wrap gap-2">
						{#each ['nsave', 'Ironbridge', 'Lemni', 'DiligenceSquared'] as company}
							<span class="inline-block bg-[#f5f5f5] text-[#555555] px-2 py-1 text-sm">{company}</span>
						{/each}
					</div>
				</div>

				<!-- Enterprise -->
				<div>
					<h3 class="text-[0.7rem] font-medium uppercase tracking-wider text-[#aaaaaa] mb-3">Enterprise</h3>
					<div class="flex flex-wrap gap-2">
						{#each ['Build', 'Fleet', 'Commerce Systems', 'Documenso'] as company}
							<span class="inline-block bg-[#f5f5f5] text-[#555555] px-2 py-1 text-sm">{company}</span>
						{/each}
					</div>
				</div>

				<!-- Healthcare & Hardware -->
				<div>
					<h3 class="text-[0.7rem] font-medium uppercase tracking-wider text-[#aaaaaa] mb-3">Healthcare & Hardware</h3>
					<div class="flex flex-wrap gap-2">
						{#each ['Medra', 'Nolla', 'Sensmore', 'Guided Energy'] as company}
							<span class="inline-block bg-[#f5f5f5] text-[#555555] px-2 py-1 text-sm">{company}</span>
						{/each}
					</div>
				</div>

				<!-- Consumer -->
				<div>
					<h3 class="text-[0.7rem] font-medium uppercase tracking-wider text-[#aaaaaa] mb-3">Consumer</h3>
					<div class="flex flex-wrap gap-2">
						{#each ['Morphic', 'Lapel', 'Hero', 'Popcorn', 'Era'] as company}
							<span class="inline-block bg-[#f5f5f5] text-[#555555] px-2 py-1 text-sm">{company}</span>
						{/each}
					</div>
				</div>
			</div>
		</section>

		<!-- How We Work -->
		<section class="mb-20 md:mb-28">
			<h2 class="text-xs font-medium uppercase tracking-widest text-[#bbbbbb] mb-6">How We Work</h2>
			<div class="grid grid-cols-1 md:grid-cols-3 gap-6 md:gap-8">
				<div>
					<h3 class="text-[1rem] font-medium text-[#333333] mb-2">Hands-on design</h3>
					<p class="text-[0.95rem] text-[#888888] leading-[1.55]">Product development partnerships, not consulting. Thilo works directly with your team on what ships.</p>
				</div>
				<div>
					<h3 class="text-[1rem] font-medium text-[#333333] mb-2">Strategic guidance</h3>
					<p class="text-[0.95rem] text-[#888888] leading-[1.55]">Pattern recognition from 40+ companies helps you avoid common pitfalls and accelerate decisions.</p>
				</div>
				<div>
					<h3 class="text-[1rem] font-medium text-[#333333] mb-2">Network access</h3>
					<p class="text-[0.95rem] text-[#888888] leading-[1.55]">Connections to Uncommon portfolio, Sequoia Arc founders, and Airbnb alumni network.</p>
				</div>
			</div>
		</section>

		<!-- Contact -->
		<section class="pt-8 border-t border-[#eeeeee]">
			<h2 class="text-xs font-medium uppercase tracking-widest text-[#bbbbbb] mb-4">Connect</h2>
			<p class="text-[1.05rem] text-[#666666] mb-6">
				Working on something early? Reach out anytime.
			</p>
			<div class="flex flex-wrap gap-3">
				<a href="https://x.com/thilokonzok" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 bg-[#111] text-white px-4 py-2.5 text-sm font-medium hover:bg-[#333] transition-colors">
					X / Twitter
				</a>
				<a href="https://linkedin.com/in/konzok" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 border border-[#dddddd] text-[#444444] px-4 py-2.5 text-sm font-medium hover:border-[#999999] hover:text-[#111] transition-colors">
					LinkedIn
				</a>
			</div>
		</section>

	</main>

	<!-- Footer -->
	<footer class="mt-20 md:mt-32 pt-8 border-t border-[#eeeeee]">
		<div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4">
			<div class="text-[#cccccc] text-sm">
				Thilo Konzok
			</div>
			<div class="text-[#cccccc] text-sm">
				San Francisco · unc.mn
			</div>
		</div>
	</footer>
</div>

