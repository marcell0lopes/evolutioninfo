<script>
	import mercadolivre from '$lib/icons/mercado-livre.svg';
	import shopee from '$lib/icons/shopee.svg';
	import b2w from '$lib/icons/b2w.svg';

	import Saos from 'saos';
</script>

<section id="vendas">
	<h2>Nossos canais de <strong>vendas</strong> online</h2>
	<div class="links">
		<Saos animation={'slide-in 0.2s cubic-bezier(0.250, 0.460, 0.450, 0.940) both'}>
			<a href="https://www.mercadolivre.com.br" target="_blank">
				<img src={mercadolivre} height={100} width={100} alt="Mercado Livre" />
			</a>
		</Saos>
		<Saos animation={'slide-in 0.2s cubic-bezier(0.250, 0.560, 0.450, 0.940) 0.1s both'}>
			<a href="https://shopee.com.br" target="_blank">
				<img src={shopee} height={100} width={100} alt="Shopee" />
			</a>
		</Saos>
		<Saos animation={'slide-in 0.2s cubic-bezier(0.250, 0.460, 0.450, 0.940) 0.2s both'}>
			<a href="http://venda.b2wmarketplace.com.br" target="_blank">
				<img src={b2w} height={100} width={100} alt="B2W" />
			</a>
		</Saos>
	</div>
</section>

<style>
	#vendas {
		margin: 0;
		padding: 2rem 1rem;
		background-color: var(--primary-color);
		background-image: linear-gradient(to bottom, rgba(24, 138, 188, 0.72), rgba(27, 46, 76, 0.93)),
			url('https://images.unsplash.com/photo-1541143273445-ba930ada04d6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1475&q=80');
		background-position: center;
		background-size: cover;
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

	.links a img {
		transition: all 0.1s ease-in-out;
	}

	.links a img:hover {
		transform: scale(1.2);
		transition: all 0.1s ease-in-out;
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
