<script>
	export let name = '';
</script>

<div class="card-container">
	<p>{name}</p>
</div>

<style>
	.card-container {
		display: flex;
		align-items: center;
		justify-content: center;
		border: 2px solid #0091ea;
		border-radius: 16px;
		color: #0091ea;
		background-color: white;
		padding: 1rem 2rem;
		margin: 0.5rem;
		box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
		transition: transform 0.3s ease;
		cursor: pointer;
		font-weight: bold;
		width:50vw;
		height: 3vh;
	}

	.card-container:hover {
		transform: translateY(-5px);
		box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
	}
</style>
