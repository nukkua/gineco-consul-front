<script>
	import FooterCards from './FooterCards.svelte';

	let footerOptions = ['Nuestros Servicios', 'Donde estamos', 'Contacto'];
</script>

<div class="footer-card">
	{#each footerOptions as option}
		<FooterCards name={option} />
	{/each}
</div>

<style>
	.footer-card {
		display: flex;
		flex-direction: column;
		align-items: center;

	}
</style>
