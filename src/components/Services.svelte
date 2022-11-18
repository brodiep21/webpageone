<script>
    // import {fade} from 'svelte/transition'
    import devpic from '../img/devpic.svg'

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
        <div class="picture">
            <div class="picture2"><img src={devpic} alt="illustration of developer"></div>
        </div>
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
    min-height:25rem;
}
.services1 h1 {
    font-size: 4rem;
    offset: left 5px;
}
.services2 {
    width: 40%;
    background-color: var(--red);
}
.picture {
    width: 70%;
    /* overflow: hidden; */
}
.picture2 {
    width: 40%;
    margin-left: 75%;
    padding-top: 1.6rem;
}
.picture img{
    background-color: var(--white);
    border-radius: 5rem;
    box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.26);
    height: 350px;
    background-size: cover;
    background-repeat: no-repeat;
    transition: .3s ease-in-out;
    position:relative;
    z-index: 6;
    
}

/* .picture:hover + .background{
    background-color: var(--black);
    width: 100px;
} */

/* <-----------------PHONE-------------> */
@media screen and (max-width: 650px) {
    .services {
        padding-left: 5px;
    }
    .services h1 {
        font-size: 39px;
    }
    .picture {
        /* text-align: left; */
        padding-top: 1rem;
    }
    .picture2 {
        margin-left: 0px;
    }
    .picture img {
        height: 175px;
    }
}

/* <---------------SMALLER SCREEN -----------> */
@media screen and (min-width: 650px) and (max-width: 1050px) {
    .picture {
        /* text-align: left; */
        padding-top: 1.6rem;
    }
    .picture2 {
        margin-left: 40%;
    }
    .picture img {
        height: 300px;
    }
}
</style>

