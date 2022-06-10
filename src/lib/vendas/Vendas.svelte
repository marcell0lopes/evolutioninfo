<script>
	import mercadolivre from '$lib/icons/mercado-livre.svg';
	import shopee from '$lib/icons/shopee.svg';
	import b2w from '$lib/icons/b2w.svg';
	import compraSegura from '$lib/icons/selo-compra-segura.png';
</script>

<section id="vendas">
	<h2>Nossos canais de <strong>vendas</strong> online</h2>
	<div class="links">
		<a href="/mercadolivre">
			<img src={mercadolivre} height={100} width={100} alt="Mercado Livre" />
		</a>
		<a href="/mercadolivre">
			<img src={shopee} height={100} width={100} alt="Shopee" />
		</a>
		<a href="/mercadolivre">
			<img src={b2w} height={100} width={100} alt="B2W" />
		</a>
		<!-- <img src={compraSegura} height={100} alt="Compra 100% Segura" /> -->
	</div>
</section>

<style>
	#vendas {
		margin: 0;
		padding: 0 1rem;
		background-color: var(--primary-color);
		margin-top: 4rem;
	}

	#vendas .links {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		align-items: center;
		margin: 2rem;
		transition: all 0.2s ease-in;
	}
	.links a {
		margin: 1rem;
	}
	.links a:hover {
		transform: scale(1.2);
		transition: all 0.2s ease-in;
	}

	#vendas h2 {
		text-align: center;
		font-size: 2rem;
		margin-top: 4rem;
		color: var(--pure-white);
	}

	@media (min-width: 720px) {
		#vendas .links {
			max-width: 800px;
			margin: 1rem auto;
			flex-direction: row;
		}
	}
</style>
