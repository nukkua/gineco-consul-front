<script>
    export let serviceTitle = '',
    serviceImg = '',
    alternativeName = '';
</script>

<div class="service-card">
    <h4>{serviceTitle}</h4>
    <div class="service-card-img">
        <img src={serviceImg} alt={alternativeName}>
    </div>
</div>

<style>
    .service-card{
        width: 250px;
        height: 300px;
        border-radius: 8%;
        border: 1px solid #0091EA;
    }
    .service-card h4{
        font-weight: bold;
        font-size: 18px;
        padding-top: 15px;
        display: flex;
        justify-content: center;
    }
    .service-card-img{
        padding-top: 25px;
        display: flex;
        align-items: center;
        justify-content: center;
    }
</style>