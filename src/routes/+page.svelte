<script>
	import BookADate from '../components/BookADate/BookADate.svelte';
	import WhoAreWe from '../components/WhoAreWe/WhoAreWe.svelte';
	import OurServices from '../components/OurServices/Service.svelte';
</script>

<main>
	<OurServices/>
	<WhoAreWe/>
</main>

<style>
	main {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		margin-left: -15rem;
	}

	@media (max-width: 768px) {
		main {
			margin-left: 0;
		}
	}
</style>
