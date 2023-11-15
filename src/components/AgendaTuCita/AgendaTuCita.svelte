<script>
	import InformationCard from '../InformationCard.svelte';
	import OptionCard from './OptionCard.svelte';
	let options = [
		{
			id: 1,
			optionName: 'Descarga nuestra app',
			alternativeName: 'Appstore and Google Play Logo',
			imageSource: '/static/images/app.png'
		},
		{
			id: 2,
			optionName: 'Escribenos',
			alternativeName: 'Whatsapp logo',
			imageSource: '/static/images/whatsapp.png'
		},
		{
			id: 1,
			optionName: 'Llamanos al +591 69409792',
			alternativeName: 'telephone logo',
			imageSource: '/static/images/telephone.png'
		}
	];
</script>

<InformationCard name="Agenda tu cita" />
<h4>Estamos aqui para ti, con 3 opciones para agendar</h4>
{#each options as option(option.id)}
	<OptionCard imageSource={option.imageSource} optionName={option.optionName} alternativeName={option.alternativeName}/>
{/each}
