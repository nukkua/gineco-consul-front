<script>
	import InformationCard from '../InformationCard.svelte';
	import OptionCard from './OptionCard.svelte';
	let options = [
		{
			id: 1,
			optionName: 'Descarga nuestra app',
			alternativeName: 'Appstore and Google Play Logo',
			imageSource: '/images/app.png'
		},
		{
			id: 2,
			optionName: 'Escribenos',
			alternativeName: 'Whatsapp logo',
			imageSource: '/images/whatsapp.png'
		},
		{
			id: 1,
			optionName: 'Llamanos al +591 69409792',
			alternativeName: 'telephone logo',
			imageSource: '/images/telephone.png'
		}
	];
</script>

<main>
	<div class="name-description">
		<InformationCard name="AGENDA TU CITA" />
		<h4>Estamos aqui para ti, con 3 opciones para agendar</h4>
	</div>
	<div>
		{#each options as option (option.id)}
			<OptionCard
				imageSource={option.imageSource}
				optionName={option.optionName}
				alternativeName={option.alternativeName}
			/>
		{/each}
	</div>
</main>

<style>
	main {
		display: flex;
		flex-direction: row;
	}
	main .name-description {
		justify-items: center;
		align-items: center;
	}
		
</style>
