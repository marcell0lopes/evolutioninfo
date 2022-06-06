<script>
	import { page } from '$app/stores';
	import logo from './svelte-logo.svg';
	import heroImage from '$lib/hero-image.jpg';
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
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg>
		<ul>
			<li class:active={$page.url.pathname === '/'}><a sveltekit:prefetch href="/">Home</a></li>
			<li class:active={$page.url.pathname === '/#quem-somos'}>
				<a sveltekit:prefetch href="#quem-somos">Quem Somos</a>
			</li>
			<li class:active={$page.url.pathname === '/#vendas'}>
				<a sveltekit:prefetch href="/#vendas">E-commerce</a>
			</li>
			<li class:active={$page.url.pathname === '/como-chegar'}>
				<a sveltekit:prefetch href="/como-chegar">Como Chegar</a>
			</li>
			<li class:active={$page.url.pathname === '/contato'}>
				<a sveltekit:prefetch href="/contato">Contato</a>
			</li>
		</ul>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav>

	<div class="corner">
		<ul>
			<li>
				<a href="https://api.whatsapp.com/send?phone=5511942086002"> whats*</a>
			</li>
			<li>
				<a href="https://www.instagram.com/evolutioninfo/"> insta*</a>
			</li>
			<li>
				<a href="https://www.facebook.com/evolution.assistance/"> face*</a>
			</li>
			<li>
				<a href="/insta"> ML*</a>
			</li>
		</ul>
	</div>
</header>

<picture>
	<img
		src={heroImage}
		class="heroImage"
		alt="Servers Informática: Peças, assistência e acessórios para seu smartphone, tablet, computador ou notebook."
	/>
</picture>

<style>
	.corner ul a {
		color: #111;
		text-decoration: underline;
		cursor: pointer;
	}

	.corner ul a:hover {
		color: #555;
	}

	header {
		z-index: 1;
		display: flex;
		justify-content: space-between;
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
		z-index: inherit;
		display: flex;
		justify-content: center;
		--background: rgba(255, 255, 255, 0.7);
	}

	svg {
		z-index: inherit;
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
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
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li.active::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--accent-color);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 1em;
		color: var(--heading-color);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	nav a:hover {
		color: var(--accent-color);
	}

	.heroImage {
		margin-top: -4.2rem;
		width: 100%;
		z-index: 0;
	}
</style>
