<script>
	import InformationCard from './InformationCard.svelte';

	let nameInformationCard = [
		'Quienes somos?',
		'Nuestros Servicios',
		'Sexinformacion',
		'Encuentranos'
	];
</script>

<header>
	<nav>
		<img src="/images/consultorioicon.png" alt="icon del consultorio" />
		{#each nameInformationCard as name}
			<InformationCard {name} />
		{/each}
	</nav>
</header>

<style>
	header {
		display: flex;
		justify-content: center;
		align-items: center;
		justify-content: space-evenly;
		margin-top: 1.5rem;
		margin-bottom: 2rem;
		height: auto;
	}
	nav {
		display: flex;
		align-items: center;
		gap: 1rem;
	}
	img {
		width: 11rem;
		height: auto;
		margin-right: 10rem;
	}
</style>
