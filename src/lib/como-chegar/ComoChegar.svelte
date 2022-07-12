<script>
	import Icon from 'svelte-awesome';
	import Saos from 'saos';
	import whatsapp from 'svelte-awesome/icons/whatsapp';
	import heart from 'svelte-awesome/icons/heart';
	import signal from 'svelte-awesome/icons/signal';
	import gears from 'svelte-awesome/icons/gears';
</script>

<section id="como-chegar">
	<div>
		<h2>O que já fizemos e onde estamos</h2>
		<ul>
			<Saos animation={'bounce-left 0.8s both;'}>
				<li>
					<Icon data={signal} scale={2} style="color: var(--primary-color);" />
					<div>
						<h3>+50.000</h3>
						<p>Vendas</p>
					</div>
				</li>
			</Saos>
			<Saos animation={'bounce-left 0.8s 0.4s both;'}>
				<li>
					<Icon data={gears} scale={2} style="color: var(--primary-color);" />
					<div>
						<h3>+45.000</h3>
						<p>Consertos</p>
					</div>
				</li>
			</Saos>
			<Saos animation={'bounce-left 0.8s 0.8s both;'}>
				<li>
					<Icon data={heart} scale={2} style="color: var(--primary-color);" />
					<div>
						<h3>+95.000</h3>
						<p>Clientes Satisfeitos</p>
					</div>
				</li>
			</Saos>
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
			title="Evolution Info"
			id="mapaGoogle"
			src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3655.3363950989506!2d-46.552198!3d-23.628120999999997!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94ce5d297468b3a9%3A0x550fe8f2d1851d2!2sEvolution%20Inform%C3%A1tica!5e0!3m2!1spt-BR!2sbr!4v1655321678024!5m2!1spt-BR!2sbr"
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

	@keyframes -global-bounce-left {
		0% {
			-webkit-transform: translateX(-48px);
			transform: translateX(-48px);
			-webkit-animation-timing-function: ease-in;
			animation-timing-function: ease-in;
			opacity: 1;
		}
		24% {
			opacity: 1;
		}
		40% {
			-webkit-transform: translateX(-26px);
			transform: translateX(-26px);
			-webkit-animation-timing-function: ease-in;
			animation-timing-function: ease-in;
		}
		65% {
			-webkit-transform: translateX(-13px);
			transform: translateX(-13px);
			-webkit-animation-timing-function: ease-in;
			animation-timing-function: ease-in;
		}
		82% {
			-webkit-transform: translateX(-6.5px);
			transform: translateX(-6.5px);
			-webkit-animation-timing-function: ease-in;
			animation-timing-function: ease-in;
		}
		93% {
			-webkit-transform: translateX(-4px);
			transform: translateX(-4px);
			-webkit-animation-timing-function: ease-in;
			animation-timing-function: ease-in;
		}
		25%,
		55%,
		75%,
		87%,
		98% {
			-webkit-transform: translateX(0px);
			transform: translateX(0px);
			-webkit-animation-timing-function: ease-out;
			animation-timing-function: ease-out;
		}
		100% {
			-webkit-transform: translateX(0px);
			transform: translateX(0px);
			-webkit-animation-timing-function: ease-out;
			animation-timing-function: ease-out;
			opacity: 1;
		}
	}
</style>
