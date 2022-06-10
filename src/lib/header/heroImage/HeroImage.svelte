<script>
	import fachadaLoja from '$lib/fachada-loja.jpg';

	import Saos from 'saos';
</script>

<section class="heroImage">
	<Saos animation={'fade-in 0.2s cubic-bezier(0.390, 0.575, 0.565, 1.000) both'}>
		<h1>Evolution Info</h1>
	</Saos>
	<Saos animation={'fade-in 1.4s cubic-bezier(0.390, 0.575, 0.565, 1.000) 1s both'}>
		<p>Peças, assistência e acessórios para seu Smartphone, Tablet, Computador ou Notebook.</p>
	</Saos>
</section>

<style>
	.heroImage {
		/* background-color: var(--secondary-color); */
		background-image: url(https://i.imgur.com/TDYmmac.jpg);
		width: 100vw;
		height: 80vh;
		overflow: -moz-hidden-unscrollable;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		text-align: center;
	}

	h1 {
		color: var(--pure-white);
		font-weight: bold;
		letter-spacing: -0.125rem;
		font-size: 4rem;
	}

	p {
		max-width: 600px;
		color: var(--tertiary-color);
		font-weight: lighter;
		letter-spacing: 0.125rem;
		font-size: 1.2rem;
	}

	@keyframes -global-fade-in {
		0% {
			-webkit-transform: translateY(-50px);
			transform: translateY(-50px);
			opacity: 0;
		}
		100% {
			-webkit-transform: translateY(0);
			transform: translateY(0);
			opacity: 1;
		}
	}
</style>
