<script>
	import fachadaLoja from '$lib/fachada-loja.jpg';
</script>

<section class="heroImage">
	<h1>Evolution Info</h1>
	<p>Peças, assistência e acessórios para seu smartphone, tablet, computador ou notebook.</p>
</section>

<style>
	.heroImage {
		/* background-color: var(--secondary-color); */
		background-image: linear-gradient(45deg, var(--primary-color), var(--secondary-color)),
			url(`fachadaLoja``);
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
</style>
