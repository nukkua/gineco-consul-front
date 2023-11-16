<script>
    export let buttonName = '',
    funtional = '';
</script>

<div class="button">
    <button  on:click={funtional} >
        {buttonName}
    </button>
</div>


<style>
    .button{
        display: flex;
        justify-content: center;
        padding-bottom: 40px;
    }
    .button button{
        height: 40px;
        width: auto;
        padding-left: 15px;
        padding-right: 15px;
        color: #F5F5F5;
        background-color: #0091EA;
        border-radius: 10px;
    }
</style>