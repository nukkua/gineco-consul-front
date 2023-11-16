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
	}

	.option-card img{
		height: 8rem;
		
	}
	.option-card h4 {
		margin-top: 5rem;
		margin-left: 2rem;
	}
</style>
