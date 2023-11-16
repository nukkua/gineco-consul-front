<script>
	export let listDepending = [];
	export let header = '';
</script>

<div class="header-list">
	<h1>{header}</h1>
	{#each listDepending as list}
		<p>{list}</p>
	{/each}
</div>

<style>
	h1 {
		font-weight: bold;
	}
	.header-list{
		display:flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin-top: 5vw;
	}
</style>
