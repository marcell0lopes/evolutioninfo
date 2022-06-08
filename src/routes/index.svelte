<script context="module">
	import QuemSomos from '../lib/quem-somos/QuemSomos.svelte';

	export const prerender = true;
</script>

<QuemSomos />

<section id="vendas">
	<h2>Nossos canais de <strong>vendas</strong> online</h2>
	ML, Shoppe, B2W, Compra segura
</section>

<section id="como-chegar">
	<h2>O que há fizemos e onde estamos</h2>
	<div>
		<ul>
			<li>
				<h3>+100.000</h3>
				<p>Vendas</p>
			</li>
			<li>
				<h3>+40.000</h3>
				<p>Consertos</p>
			</li>
			<li>
				<h3>+140.000</h3>
				<p>Clientes Satisfeitos</p>
			</li>
			<li>
				<a href="/whats">
					<button> Chamar no Whatsapp </button>
				</a>
			</li>
		</ul>
	</div>

	<div>
		<iframe
			title="Geolocalização"
			src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3655.3380872700327!2d-46.554471184422425!3d-23.62806036994528!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce5d2975226683%3A0xc37bfe75d296b46!2sR.%20Joana%20Ang%C3%A9lica%2C%20618%20-%20Barcelona%2C%20S%C3%A3o%20Caetano%20do%20Sul%20-%20SP%2C%2009551-050!5e0!3m2!1spt-BR!2sbr!4v1654541699385!5m2!1spt-BR!2sbr"
			width="600"
			height="450"
			style="border:0;"
			allowfullscreen=""
			loading="lazy"
			referrerpolicy="no-referrer-when-downgrade"
		/>
	</div>
</section>
