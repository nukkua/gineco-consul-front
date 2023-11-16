<script>
    import Title from '../Title.svelte';
    import ServiceCard from './ServiceCard.svelte';
    import Button from '../Button.svelte';
    let options = [
        {
            id: 1,
            serviceTitle: 'Consulta Ginecologica',
            serviceImg: '/images/consultaGinecologica.png',
            alternativeName: 'Consulta Ginecologica'
        },
        {
            id: 2,
            serviceTitle: 'Ecografia',
            serviceImg: '/images/ecografia.png',
            alternativeName: 'Ecografia'
        },
        {
            id: 3,
            serviceTitle: 'Papanicolaou',
            serviceImg: '/images/papanicolaou.png',
            alternativeName: 'Papanicolaou'
        }
    ];
</script>

<main>
    <Title titleName={'Nuestros Servicios'} />
    <div class="services">
        {#each options as option (option.id)}
        <div class="infividual-">
            <ServiceCard
            serviceTitle={option.serviceTitle}
            serviceImg={option.serviceImg}
            alternativeName={option.alternativeName}
            />
        </div>
        {/each}
    </div>
    <Button buttonName={'Ver todos los servicios'} funtional={''}/>
</main>

<style>
    .services{
        padding-top: 20px;
        display: flex;
        gap: 20px;
        width: auto;
		height: auto;
        padding-bottom: 50px;
    }
</style>