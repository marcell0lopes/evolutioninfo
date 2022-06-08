<script>
	import fachadaLoja from '$lib/fachada-loja.jpg';
</script>

<section class="heroImage">
	<div class="tagline">
		<h1>Evolution Info</h1>
		<p>Peças, assistência e acessórios para seu smartphone, tablet, computador ou notebook</p>
	</div>
	<img src={fachadaLoja} alt="Fachada da loja EvolutionInfo" />
</section>

<style>
	.heroImage {
		background-color: var(--secondary-color);
		width: 100vw;
		overflow: -moz-hidden-unscrollable;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.heroImage .tagline {
		margin: 0 2rem;
	}

	.heroImage h1 {
		font-weight: bold;
		font-size: 4rem;
		letter-spacing: -0.125rem;
		text-align: left;
		color: #fff;
	}

	.heroImage img {
		width: 40%;
	}

	.heroImage p {
		color: rgba(255, 255, 255, 0.9);
		font-size: 1.7rem;
	}

	@media (max-width: 600px) {
		.heroImage {
			padding: 0.2rem;
			width: 100%;
		}
		.heroImage h1 {
			text-align: center;
		}

		.heroImage {
			text-align: center;
		}

		.heroImage img {
			display: none;
		}
	}
</style>
