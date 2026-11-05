<script lang="ts">
	import BackgroundImage from '$lib/assets/bg160526.jpg';
	import InstagramLogo from '$lib/assets/insta logo.jpg';
	import TiktokLogo from '$lib/assets/tt logo.jpg';
	import YoutubeLogo from '$lib/assets/youtube logo.jpg';
</script>

<svelte:head>
	<title>Ferdi Jofer</title>
	<meta name="description" content="Ferdi Jofer - Produkte, Ideen und Alltag." />
</svelte:head>

<main class="relative min-h-screen overflow-hidden bg-black font-sans">
	<div class="background-strip absolute inset-0 flex justify-center">
		<img
			src={BackgroundImage}
			alt=""
			aria-hidden="true"
			class="background-image h-full object-cover"
		/>
		<img
			src={BackgroundImage}
			alt=""
			aria-hidden="true"
			class="background-image h-full object-cover"
		/>
		<img
			src={BackgroundImage}
			alt=""
			aria-hidden="true"
			class="background-image h-full object-cover"
		/>
	</div>

	<div
		class="relative z-10 flex min-h-screen flex-col items-center justify-end px-5 pt-16 pb-6 md:px-8 md:pb-12 lg:pb-14"
	>
		<div
			class="hero-title-wrap animate-fade-in-up relative mb-3 w-full px-5 text-center md:mb-5"
			style="animation-delay: 80ms;"
		>
			<h1 class="hero-title relative z-10 text-4xl tracking-tight text-white md:text-5xl">
				Ferdi Jofer
			</h1>
		</div>

		<div
			class="animate-fade-in-up w-full max-w-sm overflow-hidden rounded-[1.45rem] border border-white/28 bg-white/18 px-4 py-4 shadow-2xl shadow-black/18 backdrop-blur-2xl sm:max-w-xl sm:rounded-[1.5rem] md:max-w-2xl md:rounded-[1.75rem] md:px-6 md:py-5"
			style="animation-delay: 160ms;"
		>
			<div class="grid gap-4">
				<div>
					<p class="brand-intro max-w-lg text-left text-sm text-white/92 md:text-base">
						Hi, ich bin Ferdi. Ich baue mit dir coole Sachen und nehme dich ehrlich zwischen Uni,
						Gym und Alltag mit.
					</p>
				</div>
				<div class="grid gap-2">
					<a
						href="https://www.instagram.com/ideas_by_ferdi?igsh=MTA2ZG9nbzloZGdrYw%3D%3D&utm_source=qr"
						target="_blank"
						rel="noreferrer"
						aria-label="Instagram"
						class="glass-field group relative flex min-h-11 w-full items-center gap-3 px-3 py-2 overflow-hidden rounded-[0.75rem] border border-white/24 bg-white/16 text-white shadow-lg shadow-black/10 backdrop-blur-xl transition-all duration-300 focus-visible:outline-2 focus-visible:outline-white hover:border-white/55 hover:bg-white/24"
					>
						<img
							src={InstagramLogo}
							alt=""
							aria-hidden="true"
							class="relative z-10 h-6 w-6 rounded-md border border-white/30 object-cover"
						/>
						<span class="relative z-10 text-sm font-semibold">Instagram</span>
						<span aria-hidden="true" class="ml-auto text-white/75">&#8599;</span>
					</a>

					<a
						href="https://www.tiktok.com/@ideas_by_ferdi?_r=1&_t=ZG-965CN4Hk6Xg"
						target="_blank"
						rel="noreferrer"
						aria-label="TikTok"
						class="glass-field group relative flex min-h-11 w-full items-center gap-3 px-3 py-2 overflow-hidden rounded-[0.75rem] border border-white/24 bg-white/16 text-white shadow-lg shadow-black/10 backdrop-blur-xl transition-all duration-300 focus-visible:outline-2 focus-visible:outline-white hover:border-white/55 hover:bg-white/24"
					>
						<img
							src={TiktokLogo}
							alt=""
							aria-hidden="true"
							class="relative z-10 h-6 w-6 rounded-md border border-white/30 object-cover"
						/>
						<span class="relative z-10 text-sm font-semibold">TikTok</span>
						<span aria-hidden="true" class="ml-auto text-white/75">&#8599;</span>
					</a>

					<a
						href="https://www.youtube.com/channel/UC0N4NlvsjdYbBUtISf8GVIA"
						target="_blank"
						rel="noreferrer"
						aria-label="YouTube"
						class="glass-field group relative flex min-h-11 w-full items-center gap-3 px-3 py-2 overflow-hidden rounded-[0.75rem] border border-white/24 bg-white/16 text-white shadow-lg shadow-black/10 backdrop-blur-xl transition-all duration-300 focus-visible:outline-2 focus-visible:outline-white hover:border-white/55 hover:bg-white/24"
					>
						<img
							src={YoutubeLogo}
							alt=""
							aria-hidden="true"
							class="relative z-10 h-6 w-6 rounded-md border border-white/30 object-cover"
						/>
						<span class="relative z-10 text-sm font-semibold">YouTube</span>
						<span aria-hidden="true" class="ml-auto text-white/75">&#8599;</span>
					</a>
				</div>
			</div>

		</div>

		<p
			class="animate-fade-in-up mt-3 text-center text-[11px] font-semibold text-white drop-shadow-[0_2px_10px_rgba(0,0,0,0.45)] md:text-sm"
			style="animation-delay: 220ms;"
		>
			© 2026 Ferdi Jofer. Alle Rechte vorbehalten.
		</p>
	</div>
</main>

<style>
	@keyframes fade-in-up {
		from {
			opacity: 0;
			transform: translateY(20px);
		}
		to {
			opacity: 1;
			transform: translateY(0);
		}
	}

	.animate-fade-in-up {
		animation: fade-in-up 0.6s ease-out forwards;
		opacity: 0;
	}

	.brand-intro {
		font-family: var(--font-sans);
		font-weight: 430;
		letter-spacing: 0.003em;
		line-height: 1.45;
	}

	.background-strip {
		top: -3%;
		bottom: 0;
		min-width: 100vw;
	}

	.background-image {
		flex: 0 0 auto;
		width: auto;
		filter: none;
	}


	@media (max-width: 767px) {
		.background-strip {
			top: -5%;
			bottom: 0;
			left: 50%;
			min-width: auto;
			transform: translateX(-50%);
		}

		.background-image {
			display: none;
			width: auto;
			max-width: none;
		}

		.background-image:nth-child(2) {
			display: block;
			height: 100%;
			object-position: center 44%;
		}
	}

	.hero-title-wrap::before {
		content: '';
		position: absolute;
		top: 50%;
		left: 50%;
		width: min(74vw, 34rem);
		height: 8rem;
		background: rgba(0, 0, 0, 0.34);
		border-radius: 999px;
		filter: blur(44px);
		transform: translate(-50%, -50%);
	}

	.hero-title {
		text-shadow: 0 10px 30px rgba(0, 0, 0, 0.32);
	}

	.glass-field::before {
		content: '';
		position: absolute;
		inset: 0;
		background: linear-gradient(135deg, rgba(255, 255, 255, 0.28), transparent 46%);
		opacity: 0;
		transition: opacity 0.3s ease;
	}

	.glass-field:hover::before {
		opacity: 1;
	}
</style>
