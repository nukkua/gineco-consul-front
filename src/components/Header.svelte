<script>
	import InformationCard from './InformationCard.svelte';

	let nameInformationCard = [
		'Quienes somos?',
		'Nuestros Servicios',
		'Sexinformacion',
		'Encuentranos'
	];

	let isMenuOpen = false;
</script>

<header>
	<img src="/images/consultorioicon.png" alt="icon del consultorio" />
	<nav class:open={isMenuOpen}>
		{#each nameInformationCard as name}
			<InformationCard {name} />
		{/each}
	</nav>

	<button
		on:click={() => {
			isMenuOpen = !isMenuOpen;
			console.log('Menu Open:', isMenuOpen); // Agrega esto para depurar
		}}
		class="hamburger-button">☰</button
	>
</header>

<style>
	header {
		display: flex;
		height: auto;
		margin-top: 3vh;
		justify-content: center;
		align-items: center;
	}

	nav {
		align-items: center;
		display: flex;
		gap: 0.5rem;
	}

	img {
		margin-left: 5vw;
		margin-right: 5vw;
		max-width: 100%;
		height: auto;
		object-fit: contain;
	}

	.hamburger-button {
		display: none;
		font-size: 2rem;
		color: black;
	}

	@media (max-width: 769px) {
		header {
			flex-direction: column;
			justify-content: center;
			align-items: center;
		}
		.hamburger-button {
			display: block; 
		}

		nav {
			display: none; 
		}

		nav.open {
			display: flex; 
			flex-direction: column;
			align-items: center;
		}
	}
</style>
