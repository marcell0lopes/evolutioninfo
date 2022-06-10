<script>
	import logo from './svelte-logo.svg';

	import Icon from 'svelte-awesome';
	import whatsapp from 'svelte-awesome/icons/whatsapp';
	import instagram from 'svelte-awesome/icons/instagram';
	import facebook from 'svelte-awesome/icons/facebook';
	import mercadolivre from '$lib/icons/mercadolivre.svg';
	import HeroImage from './heroImage/HeroImage.svelte';
</script>

<!-- <section class="useful-links">
	<div>
		<a
			target="_blank"
			href="https://www.google.com/maps/place/R.+Joana+Ang%C3%A9lica,+618+-+Barcelona,+S%C3%A3o+Caetano+do+Sul+-+SP,+09551-050/@-23.6280604,-46.5544712,17z/data=!4m13!1m7!3m6!1s0x94ce5d2975226683:0xc37bfe75d296b46!2sR.+Joana+Ang%C3%A9lica,+618+-+Barcelona,+S%C3%A3o+Caetano+do+Sul+-+SP,+09551-050!3b1!8m2!3d-23.6280653!4d-46.5522825!3m4!1s0x94ce5d2975226683:0xc37bfe75d296b46!8m2!3d-23.6280653!4d-46.5522825"
		>
			Rua Joana Angélica, 618 09551-050 São Caetano do Sul, SP
		</a>
	</div>
	<div>
		<a href="https://api.whatsapp.com/send?phone=5511942086002"> whats*</a>
		<a href="https://www.instagram.com/evolutioninfo/"> insta*</a>
		<a href="https://www.facebook.com/evolution.assistance/"> face*</a>
		<a href="/insta"> ML*</a>
	</div>
</section> -->

<header>
	<div class="corner">
		<a href="/">
			<img src={logo} alt="SvelteKit" />
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
				<a target="_blank" href="/#">
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
		background: #02679b;
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
