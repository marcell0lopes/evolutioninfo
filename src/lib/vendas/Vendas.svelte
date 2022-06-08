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
		<img src={compraSegura} height={100} alt="Compra 100% Segura" />
	</div>
</section>

<style>
	#vendas {
		margin: 0;
		width: 100%;
	}

	#vendas .links {
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin: 4rem 0;
		transition: all 0.2s ease-in;
	}

	.links a:hover {
		transform: scale(1.2);
		transition: all 0.2s ease-in;
	}

	#vendas h2 {
		text-align: center;
		font-size: 2rem;
		margin-top: 6rem;
		color: var(--primary-color);
	}
</style>
