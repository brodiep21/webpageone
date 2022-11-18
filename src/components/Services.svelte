<script>
    // import {fade} from 'svelte/transition'
    import {devpic} from '../img/devpic.svg'

    // const picture = [
    //     '../img/devpic.svg',
    //     '../img/devpic2.svg',
    //     '../img/devpic3.svg'
    // ];


</script>
                                                                                       
<section class="servicesection" href=#services id="services">
    <div class="services">
        <div class="services1">
            <h3>Fit your needs</h3>
            <h1>My <br> Services.</h1>
        </div>
        <div class="picture"><img src={devpic} alt="illustration of developer"></div>
        <div class="services2"></div>
    </div>
    
    <!-- <div class="background"></div> -->
</section>

<style>

.servicesection {
    display: flex;
}
.services {
    background: var(--lorange);
    width: 100%;
    display: flex;
}
.services1 h1 {
    font-size: 4rem;
    offset: left 5px;
}
.background {
    width: 100%;

}
.picture {
    width: 100px;
}
.picture img{
    background-size: contain;
    background-repeat: no-repeat;
    transition: .3s ease-in-out;
    height: 80px;
    width: 80px;
}
/* .picture:hover + .background{
    background-color: var(--black);
    width: 100px;
} */

@media screen and (max-width: 650px) {
    .services {
        padding-left: 5px;
    }
    .services h1 {
        font-size: 39px;
    }
}
</style>

