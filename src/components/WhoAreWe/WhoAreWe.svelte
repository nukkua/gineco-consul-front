<script>
	import Title from '../Title.svelte';
	import ButtonWhoAreWe from './ButtonWhoAreWe.svelte';
	import DescriptionWhoAreWe from './DescriptionWhoAreWe.svelte';
</script>

<div class="main-container">
	<Title titleName={'Quienes somos?'} />
	<div class="information-image">
		<img src="/images/WhoAreWeImage.png" alt="" />
		<div class="information">
			<DescriptionWhoAreWe />
			<ButtonWhoAreWe />
		</div>
	</div>
</div>

<style>
	.main-container {
		display: flex;
		flex-direction: column;
		align-content: center;
		justify-content: center;
	}
	.main-container .information-image img{
		width: 50vw;
		height: 50hw;
		margin-left: 25vw;
	}
	@media (min-width: 769px) {
		.main-container {
			display: flex;
			align-content: center;
			justify-content: center;
		}
		.main-container .information-image{
			display:flex;
			flex-direction: row;
			margin-left: -13vw;
		}
		.main-container .information-image img {
			width: 15vw;
			height: auto;
		}
		.information {
			margin-left: 5vw;
		}

	}
</style>
