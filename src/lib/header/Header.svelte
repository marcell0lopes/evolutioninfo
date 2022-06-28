<script>
	import Icon from 'svelte-awesome';
	import whatsapp from 'svelte-awesome/icons/whatsapp';
	import instagram from 'svelte-awesome/icons/instagram';
	import facebook from 'svelte-awesome/icons/facebook';
	import mercadolivre from '$lib/icons/mercadolivre.svg';
	import HeroImage from './heroImage/HeroImage.svelte';
	import logo from './globo.png';
</script>

<header>
	<div class="corner">
		<a href="/">
			<img src={logo} id="navLogo" alt="SvelteKit" />
		</a>
	</div>

	<nav>
		<ul>
			<li><a sveltekit:prefetch href="/">Home</a></li>
			<li>
				<a sveltekit:prefetch href="#quem-somos">Quem Somos</a>
			</li>
			<li>
				<a sveltekit:prefetch href="/#vendas">E-commerce</a>
			</li>
			<li>
				<a sveltekit:prefetch href="/#como-chegar">Como Chegar</a>
			</li>
			<li>
				<a sveltekit:prefetch href="/#contato">Contato</a>
			</li>
		</ul>
	</nav>

	<div class="corner">
		<ul>
			<li>
				<a target="_blank" href="https://api.whatsapp.com/send?phone=5511942086002">
					<Icon data={whatsapp} label="Whatsapp" style="color: #fff;" />
				</a>
			</li>
			<li>
				<a target="_blank" href="https://www.instagram.com/evolutioninfo/">
					<Icon data={instagram} label="Instagram" style="color: #fff;" />
				</a>
			</li>
			<li>
				<a target="_blank" href="https://www.facebook.com/evolution.assistance/">
					<Icon data={facebook} label="Facebook" style="color: #fff;" />
				</a>
			</li>
			<li>
				<a target="_blank" href="https://www.mercadolivre.com.br/perfil/EVOLUTION_MIX">
					<img src={mercadolivre} alt="Mercado Livre" class="filter-white" />
				</a>
			</li>
		</ul>
	</div>
</header>

<HeroImage />

<style>
	.filter-white {
		filter: invert(99%) sepia(0%) saturate(0%) hue-rotate(59deg) brightness(112%) contrast(100%);
	}
	.corner ul a {
		color: #111;
		text-decoration: underline;
		cursor: pointer;
		margin-left: 1rem;
	}

	.corner ul a:hover {
		color: #555;
	}

	header {
		z-index: 1;
		display: flex;
		align-items: center;
		justify-content: space-between;
		width: 100%;
		height: 4rem;
		background: #044d85;
	}

	#navLogo {
		width: fit-content;
	}

	.corner {
		width: 12em;
		height: 3em;
		z-index: 1;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	}

	nav {
		--background: rgba(255, 255, 255, 0.7);
		z-index: inherit;
		display: flex;
		justify-content: center;
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
	}

	li {
		position: relative;
		height: 100%;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 1rem;
		color: var(--pure-white);
		font-weight: bold;
		font-size: 0.85rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	nav a:hover {
		color: var(--accent-color);
	}

	@media (max-width: 600px) {
		nav {
			display: none;
		}
	}
</style>
