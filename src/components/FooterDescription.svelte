<script>
	let services = ['Consulta ginecologica', 'Ecografias', 'Papanicolau', 'Control Prenatal'];
	let whoAreWe = ['Historia', 'Mision', 'Ubicacion'];
	let utils = ['Quienes somos', 'Nuestro Trabajo', 'Contacto'];
	import FooterDescriptions from '../components/FooterDescriptions.svelte';
</script>

<div class="footer-description">
	<FooterDescriptions header={'Nuestros Servicios'} listDepending={services} />
	<FooterDescriptions header={'Quienes Somos'} listDepending={whoAreWe} />
	<FooterDescriptions header={'Enlaces utiles'} listDepending={utils} />
</div>

<style>
	.footer-description{
		display:flex;
		flex-direction: column;
		align-items:center;
		justify-content: center;
		margin-bottom: 3vh;
	}
</style>
