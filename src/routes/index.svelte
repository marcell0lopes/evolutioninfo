<script context="module">
	export const prerender = true;
	import fachadaLoja from '$lib/fachada-loja.jpg';
</script>

<svelte:head>
	<title>EvolutionInfo</title>
	<meta
		name="description"
		content="Nossa Missão. É proporcionar aos nossos clientes o melhor atendimento com transparência no serviço prestado e eficiência no resultado. Visão. Ser a melhor loja de assistência técnica e vendas de acessórios do ABC, referência em qualidade e segurança. Valores."
	/>
</svelte:head>

<section id="quem-somos">
	<img src={fachadaLoja} alt="Fachada da loja EvolutionInfo" />
	<div>
		<h2>&bull; Quem Somos</h2>

		<h3>Nossa Missão</h3>
		<p>
			Nossa Missão É proporcionar aos nossos clientes o melhor atendimento com transparência no
			serviço prestado e eficiência no resultado.
		</p>
		<h3>Visão</h3>
		<p>
			Ser a melhor loja de assistência técnica e vendas de acessórios do ABC, referência em
			qualidade e segurança.
		</p>
		<h3>Valores</h3>
		<p>
			Tratamos todos nossos clientes de igual para igual, pois nos colocamos no lugar deles para
			atendê-los e assim resolvermos suas necessidades com zelo, atenção e carinho.
		</p>
	</div>
</section>

<section id="vendas">
	<h2>Nossos canais de <strong>vendas</strong> online</h2>
	ML, Shoppe, B2W, Compra segura
</section>

<section id="como-chegar">
	<h2>O que há fizemos e onde estamos</h2>
	<div>
		<ul>
			<li>
				<h3>+100.000</h3>
				<p>Vendas</p>
			</li>
			<li>
				<h3>+40.000</h3>
				<p>Consertos</p>
			</li>
			<li>
				<h3>+140.000</h3>
				<p>Clientes Satisfeitos</p>
			</li>
			<li>
				<a href="/whats">
					<button> Chamar no Whatsapp </button>
				</a>
			</li>
		</ul>
	</div>

	<div>
		<iframe
			title="Geolocalização"
			src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3655.3380872700327!2d-46.554471184422425!3d-23.62806036994528!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce5d2975226683%3A0xc37bfe75d296b46!2sR.%20Joana%20Ang%C3%A9lica%2C%20618%20-%20Barcelona%2C%20S%C3%A3o%20Caetano%20do%20Sul%20-%20SP%2C%2009551-050!5e0!3m2!1spt-BR!2sbr!4v1654541699385!5m2!1spt-BR!2sbr"
			width="600"
			height="450"
			style="border:0;"
			allowfullscreen=""
			loading="lazy"
			referrerpolicy="no-referrer-when-downgrade"
		/>
	</div>
</section>

<style>
	#quem-somos img {
		width: 100%;
	}

	#quem-somos h2 {
		color: var(--primary-color);
		font-size: 2rem;
		font-weight: bold;
	}

	#quem-somos h3 {
		color: var(--accent-color);
		font-size: 1.5rem;
		margin-top: 2rem;
	}

	#quem-somos p {
		color: var(--text-color);
		margin-top: -0.8rem;
		line-height: 1.6rem;
	}

	@media (min-width: 600px) {
		#quem-somos {
			display: flex;
			flex-direction: row;
			justify-content: center;
			align-items: center;
		}

		#quem-somos img {
			width: 60%;
		}

		#quem-somos div {
			background: var(--tertiary-color);
			padding: 1rem 3rem;
			margin-left: -10rem;
			width: 70%;
			height: 60%;
			filter: drop-shadow(0 5px 20px rgba(0, 0, 0, 0.2));
		}
	}
</style>
