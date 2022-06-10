<script>
	import Icon from 'svelte-awesome';
	import whatsapp from 'svelte-awesome/icons/whatsapp';
	import heart from 'svelte-awesome/icons/heart';
	import signal from 'svelte-awesome/icons/signal';
	import gears from 'svelte-awesome/icons/gears';
</script>

<section id="como-chegar">
	<div>
		<h2>O que há fizemos e onde estamos</h2>
		<ul>
			<li>
				<Icon data={signal} scale={2} style="color: var(--primary-color);" />
				<div>
					<h3>+100.000</h3>
					<p>Vendas</p>
				</div>
			</li>
			<li>
				<Icon data={gears} scale={2} style="color: var(--primary-color);" />
				<div>
					<h3>+40.000</h3>
					<p>Consertos</p>
				</div>
			</li>
			<li>
				<Icon data={heart} scale={2} style="color: var(--primary-color);" />
				<div>
					<h3>+140.000</h3>
					<p>Clientes Satisfeitos</p>
				</div>
			</li>
			<li>
				<a href="https://api.whatsapp.com/send?phone=5511942086002">
					<button>
						<Icon
							data={whatsapp}
							style="margin-right: .4rem; transform: translateY(2px); color: #fff"
						/>Chamar no Whatsapp
					</button>
				</a>
			</li>
		</ul>
	</div>
	<div>
		<iframe
			id="mapaGoogle"
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

<style>
	#como-chegar {
		padding: 0 1rem;
	}
	h2 {
		color: var(--primary-color);
		font-size: 2rem;
		font-weight: bold;
	}

	ul {
		list-style: none;
		padding: 0;
	}

	ul li {
		display: flex;
		align-items: center;
	}
	ul li div {
		margin-left: 1.5rem;
	}

	ul li h3 {
		color: var(--primary-color);
		font-size: 1.5rem;
		font-weight: bold;
	}

	ul li p {
		color: var(--text-color);
		font-size: 1rem;
		margin-top: -1.4rem;
		margin-bottom: 1.8rem;
	}

	ul button {
		padding: 0.5rem 1.25rem;
		background-color: var(--primary-color);
		color: var(--tertiary-color);
		font-weight: bold;
		border-radius: 0.5rem;
		border: none;
	}

	#mapaGoogle {
		margin: 1rem;
		max-width: 90%;
	}

	@media (min-width: 720px) {
		#como-chegar {
			margin: 0 auto;
			max-width: 1024px;
			display: flex;
			align-items: center;
		}

		#como-chegar div:first-child {
			padding: 1rem;
		}
	}
</style>
