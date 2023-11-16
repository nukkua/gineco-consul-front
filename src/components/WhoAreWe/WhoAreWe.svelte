<script>
	import Title from '../Title.svelte';
	import ButtonWhoAreWe from './ButtonWhoAreWe.svelte';
	import DescriptionWhoAreWe from './DescriptionWhoAreWe.svelte';
</script>

<div class="main-container">
	<Title titleName={'Quienes somos?'} />
	<img src="/images/WhoAreWeImage.png" alt="" />
	<div class="information">
		<DescriptionWhoAreWe />
		<ButtonWhoAreWe />
	</div>
</div>

<style>
	.main-container {
		display: flex;
		flex-direction: column;
		align-content: center;
		justify-content: center;
	}
	.main-container img {
		width: 40vw;
		height: 40hw;
		align-content: center;
		justify-content: center;
	}
</style>
