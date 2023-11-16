<script>
	export let name = '';
</script>

<button>{name}</button>


<style>
    button {
        width: 9rem;
        height: 3rem;
        color: #1387ec;
        background-color: rgba(19, 135, 236, 0.12);
        margin-right: 1rem;
        border-radius: 1rem;
        border: none;
    }

    @media (max-width: 768px) {
        button {
            width: 100%; /* Hace que el botón se expanda para llenar el espacio disponible */
            margin: 0.5rem 0; /* Ajuste de margen para dispositivos móviles */
        }
    }
</style>

