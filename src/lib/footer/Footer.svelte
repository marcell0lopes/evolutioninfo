<script>
	import logoGrande from './logoevolution.png';
	import Icon from 'svelte-awesome';

	import caretRight from 'svelte-awesome/icons/caretRight';
	import whatsapp from 'svelte-awesome/icons/whatsapp';
	import instagram from 'svelte-awesome/icons/instagram';
	import facebook from 'svelte-awesome/icons/facebook';
	import mercadolivre from '$lib/icons/mercadolivre.svg';
</script>

<footer>
	<div>
		<img src={logoGrande} alt="Evolution Info" class="logo" />
		<p>Assistência técnica para computadores, tablets e smartphones.</p>
	</div>

	<div class="links">
		<a href="/">
			<Icon data={caretRight} />
			<p>Home</p>
		</a>

		<a href="/#quem-somos">
			<Icon data={caretRight} />
			<p>Quem Somos</p>
		</a>

		<a href="/#vendas">
			<Icon data={caretRight} />
			<p>E-commerce</p>
		</a>

		<a href="/#como-chegar">
			<Icon data={caretRight} />
			<p>Como Chegar</p>
		</a>
	</div>

	<div class="contato">
		<h2>Entre em contato conosco</h2>
		<div class="socialMedia">
			<a target="_blank" href="https://api.whatsapp.com/send?phone=5511944720871">
				<Icon data={whatsapp} scale={2} label="Whatsapp" style="color: var(--primary-color)" />
			</a>

			<a target="_blank" href="https://www.instagram.com/evolutioninfo/">
				<Icon data={instagram} style="color: var(--primary-color)" label="Instagram" scale={2} />
			</a>

			<a target="_blank" href="https://www.facebook.com/evolution.assistance/">
				<Icon data={facebook} style="color: var(--primary-color)" label="Facebook" scale={2} />
			</a>

			<a target="_blank" href="/#">
				<img src={mercadolivre} alt="Mercado Livre" height="35px" class="filter-blue" />
			</a>
		</div>

		<p>
			(11) 4228-1646 <br />
			Whatsapp: <a href="https://api.whatsapp.com/send?phone=5511944720871">(11) 94472-0871</a>
		</p>

		<a target="_blank" href="https://goo.gl/maps/4gwmTuxwG6zATE9j8">
			Rua Joana Angélica, 618 <br /> 09551-050 - São Caetano do Sul, SP
		</a>
	</div>
</footer>

<style>
	.filter-blue {
		filter: invert(49%) sepia(44%) saturate(922%) hue-rotate(153deg) brightness(86%) contrast(88%);
	}
	footer {
		padding: 1.5rem 0.7rem;
		display: flex;
		flex-direction: column;
		text-align: center;
		background-color: var(--pure-white);
	}

	footer div p {
		color: var(--text-color);
		font-size: 1.2rem;
	}
	.links {
		margin: 2rem 0;
	}
	.links a {
		display: block;

		font-size: 1.2rem;
		margin: 1rem 0;
		letter-spacing: 0.15rem;
	}

	.links a p {
		display: inline;
	}

	.links a p:hover {
		cursor: pointer;
		color: var(--accent-color);
	}

	footer div h2 {
		color: var(--tertiary-color);
		font-size: 1.4rem;
		font-weight: bold;
	}

	.logo {
		max-width: 12rem;
		margin: 1rem auto;
	}

	.contato h2 {
		color: var(--accent-color);
	}

	.contato a {
		color: var(--primary-color);
	}

	.contato a:hover {
		filter: brightness(0.8);
	}

	.socialMedia {
		list-style: none;
		color: var(--primary-color);
	}
	.socialMedia a + a {
		display: inline;
		margin-left: 1rem;
	}

	@media (min-width: 720px) {
		footer {
			padding: 2rem;
			display: grid;
			grid-template-columns: repeat(3, 1fr);
			gap: 2rem;
		}
	}
</style>
