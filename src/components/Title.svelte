<script>
	export let titleName = '';
</script>

<div class="main-container">
	<h1>{titleName}</h1>
	<img src="/images/linetitle.png" alt="" />
</div>

<style>
	.main-container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin-bottom: 10px;
	}
	h1 {
		font-weight: bold;
	}
	img {
		width: 30vw;
	}
	@media(min-width: 769px){
	}
</style>
