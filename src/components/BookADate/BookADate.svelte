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
			id: 3,
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
			<div class="individual-option">
				<OptionCard
					imageSource={option.imageSource}
					optionName={option.optionName}
					alternativeName={option.alternativeName}
				/>
			</div>
		{/each}
	</div>
</main>

<style>
	main {
		display: flex;
		flex-direction: column; /* Comienza con column para mobile first */
		align-items: center; /* Centra elementos en eje cruzado */
		justify-content: center; /* Centra elementos en eje principal */
		padding: 2vh; /* Agrega padding en lugar de margen superior */
		width: 100%; /* Ocupa el ancho total */
	}

	main .name-description {
		text-align: center; /* Centra el texto para títulos y subtítulos */
		margin-bottom: 2rem; /* Espacio entre el título y las opciones */
	}

	main .individual-option {
		width: 100%; /* Ocupa el ancho total */
		margin-bottom: 1rem; /* Espacio entre opciones */
	}

	@media (min-width: 769px) {
		main {
			flex-direction: row; /* Cambia a disposición en fila para pantallas grandes */
			justify-content: center;
			align-items: center; /* Alinea los elementos al comienzo de su contenedor */

		}

		main .name-description {
			text-align: center; /* Centra el texto del título */
			order: -1; /* Asegura que el título se muestre primero */
		}

		main .individual-option {
			justify-content: center;
			align-items: center; /* Alinea los elementos al comienzo de su contenedor */
		}
	}
</style>
