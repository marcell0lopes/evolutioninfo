<script>
	import mercadolivre from '$lib/icons/mercado-livre.svg';
	import shopee from '$lib/icons/shopee.svg';
	import b2w from '$lib/icons/b2w.svg';
	import compraSegura from '$lib/icons/selo-compra-segura.png';

	import Saos from 'saos';
</script>

<section id="vendas">
	<h2>Nossos canais de <strong>vendas</strong> online</h2>
	<div class="links">
		<Saos animation={'slide-in 0.2s cubic-bezier(0.250, 0.460, 0.450, 0.940) both'}>
			<a href="/mercadolivre">
				<img src={mercadolivre} height={100} width={100} alt="Mercado Livre" />
			</a>
		</Saos>
		<Saos animation={'slide-in 0.2s cubic-bezier(0.250, 0.560, 0.450, 0.940) 0.1s both'}>
			<a href="/mercadolivre">
				<img src={shopee} height={100} width={100} alt="Shopee" />
			</a>
		</Saos>
		<Saos animation={'slide-in 0.2s cubic-bezier(0.250, 0.460, 0.450, 0.940) 0.2s both'}>
			<a href="/mercadolivre">
				<img src={b2w} height={100} width={100} alt="B2W" />
			</a>
		</Saos>
		<!-- <img src={compraSegura} height={100} alt="Compra 100% Segura" /> -->
	</div>
</section>

<style>
	#vendas {
		margin: 0;
		padding: 2rem 1rem;
		background-color: var(--primary-color);
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
		color: var(--pure-white);
		margin-bottom: 4rem;
	}

	@media (min-width: 720px) {
		#vendas .links {
			max-width: 800px;
			margin: 1rem auto;
			flex-direction: row;
		}
	}

	@keyframes -global-slide-in {
		0% {
			-webkit-transform: translateZ(-1400px) translateX(-1000px);
			transform: translateZ(-1400px) translateX(-1000px);
			opacity: 0;
		}
		100% {
			-webkit-transform: translateZ(0) translateX(0);
			transform: translateZ(0) translateX(0);
			opacity: 1;
		}
	}
</style>
