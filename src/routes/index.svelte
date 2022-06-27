<script context="module">
	import QuemSomos from '../lib/quem-somos/QuemSomos.svelte';
	import Vendas from '../lib/vendas/Vendas.svelte';
	import ComoChegar from '$lib/como-chegar/ComoChegar.svelte';
	import MercadoLider from '../lib/mercadolider/MercadoLider.svelte';

	export const prerender = true;
</script>

<QuemSomos />
<Vendas />
<ComoChegar />
<MercadoLider />
