<script>
	import fachadaLoja from '$lib/fachada-loja.jpg';
	import Saos from 'saos';
</script>

<section id="quem-somos">
	<img src={fachadaLoja} alt="Fachada da loja EvolutionInfo" />
	<div>
		<h2>&bull; Quem Somos</h2>

		<Saos animation={'swing-in 0.5s cubic-bezier(0.175, 0.885, 0.320, 1.275) both'}>
			<h3>Nossa Missão</h3>
			<p>
				Nossa Missão É proporcionar aos nossos clientes o melhor atendimento com transparência no
				serviço prestado e eficiência no resultado.
			</p>
		</Saos>
		<Saos animation={'swing-in 0.5s cubic-bezier(0.175, 0.885, 0.320, 1.275) .75s both'}>
			<h3>Visão</h3>
			<p>
				Ser a melhor loja de assistência técnica e vendas de acessórios do ABC, referência em
				qualidade e segurança.
			</p>
		</Saos>
		<Saos animation={'swing-in 0.5s cubic-bezier(0.175, 0.885, 0.320, 1.275) 1.5s both'}>
			<h3>Valores</h3>
			<p>
				Tratamos todos nossos clientes de igual para igual, pois nos colocamos no lugar deles para
				atendê-los e assim resolvermos suas necessidades com zelo, atenção e carinho.
			</p>
		</Saos>
	</div>
</section>

<style>
	#quem-somos {
		margin-top: 4rem;
		padding: 0 1rem;
	}

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
			margin: 3rem auto;
			max-width: 1024px;
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

	@keyframes -global-swing-in {
		0% {
			-webkit-transform: rotateY(100deg);
			transform: rotateY(100deg);
			-webkit-transform-origin: left;
			transform-origin: left;
			opacity: 0;
		}
		100% {
			-webkit-transform: rotateY(0);
			transform: rotateY(0);
			-webkit-transform-origin: left;
			transform-origin: left;
			opacity: 1;
		}
	}
</style>
