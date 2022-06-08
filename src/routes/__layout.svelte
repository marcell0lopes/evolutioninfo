<script>
	import Header from '$lib/header/Header.svelte';
	import Footer from '$lib/footer/Footer.svelte';
	import '../app.css';
</script>

<svelte:head>
	<title>EvolutionInfo</title>
	<meta
		name="description"
		content="Nossa Missão. É proporcionar aos nossos clientes o melhor atendimento com transparência no serviço prestado e eficiência no resultado. Visão. Ser a melhor loja de assistência técnica e vendas de acessórios do ABC, referência em qualidade e segurança. Valores."
	/>
</svelte:head>

<Header />

<main>
	<slot />
</main>

<Footer />

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>
