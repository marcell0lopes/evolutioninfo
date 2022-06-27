<script>
	import MercadoLiderPLatinum from '$lib/icons/mercado-lider-platinum.svg';
	import Compra100Segura from '$lib/icons/compra-100-segura.svg';
</script>

<section id="MercadoLider">
	<img src={MercadoLiderPLatinum} alt="Mercado Líder Platinum" />
	<img src={Compra100Segura} alt="Compra 100% Segura" />
</section>

<style>
	#MercadoLider {
		background-color: var(--primary-color);
		width: 100%;
		padding: 2rem 0;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	img {
		margin: 0 auto;
		max-width: 70%;
		max-height: 6rem;
	}

	img:first-child {
		margin-bottom: 2rem;
	}

	@media (min-width: 720px) {
		#MercadoLider {
			flex-direction: row;
			justify-content: space-around;
			padding: 4rem 0;
		}

		img:first-child {
			margin-bottom: 0;
		}
	}
</style>
