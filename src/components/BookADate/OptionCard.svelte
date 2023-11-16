<script>
	export let imageSource = '',
		optionName = '',
		alternativeName = '';
</script>

<div class="option-card">
	<img src={imageSource} alt={alternativeName} />
	<h4>{optionName}</h4>
</div>

<style>
	.option-card {
		display:flex;
		flex-direction: row;
		margin-bottom: 2rem;
	}

	.option-card img{
		height: 10vh;
		
	}
	.option-card h4 {
		margin-top: 5vh;
		margin-left: 2vw;
	}

	@media (max-width: 769px){
		.option-card img {
			height: 7vh;
		}
		.option-card h4 {
			margin-top: 2vh;
			margin-left:  3vw;
		}
	}
</style>
