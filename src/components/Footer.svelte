<script>
	import FooterCard from "./FooterCard.svelte";
	import FooterDescription from "./FooterDescription.svelte"


</script>
<div class="main-container">
	<div class="icon-ourservices">
		<FooterCard/>
		<img src="/images/consultorioicon.png" alt="Icon del consultorio">
	</div>
	<FooterDescription/>

</div>

<style>
	.main-container{
		display:flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		background-color: white;
		margin-top: 2vh;
	}
	.main-container .icon-ourservices{
		flex-direction: column;
	}
	.main-container img{
		margin-top: 2vh;
		margin-bottom: 2vh;
	}

	@media(min-width: 769px){
		.main-container{
			display:flex;
			flex-direction: row;
		}
	}

</style>
