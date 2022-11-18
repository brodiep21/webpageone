<script>
    // import {fade} from 'svelte/transition'
    import devpic from '../img/devpic3.svg'

    // const picture = [
    //     '../img/devpic.svg',
    //     '../img/devpic2.svg',
    //     '../img/devpic3.svg'
    // ];


</script>
                                                                                       
<section class="servicesection" href=#services id="services">
    <div class="services">
        <div class="services1">
            <h3>Fit Your Needs</h3>
            <h1>My <br> Services.</h1>
            <p>Your small business needs a website?  Lets get you on map, I offer a variety of choices, and can tailor to whatever your website needs.</p>
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
    margin-left: 2rem;
}
.services h3 {
    margin-left: 2rem;
    margin-top: 2rem;
    font-family:'Courier New', Courier, monospace;
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
    margin-left: 70%;
    padding-top: 1.6rem;
    
    overflow:visible;
}
.picture img{
    background-color: var(--white);
    border-radius: 5rem;
    box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.26);
    height: 400px;
    width: auto;
    background-size: cover;
    background-repeat: no-repeat;
    transition: .3s ease-in-out;
    position:relative;
    z-index: 1;
    
}

/* .picture:hover + .background{
    background-color: var(--black);
    width: 100px;
} */

/* <-----------------PHONE/SMALL SCREEN-------------> */
@media screen and (max-width: 850px) {
    .services {
        padding-left: 5px;
    }
    .services h1 {
        font-size: 39px;
    }
    .services2 {
    width: 60%;
}
    .picture {
        width: 40%;
        padding-top: 1rem;
    }
    .picture2 {
        margin-left: 0px;
    }
    .picture img {
        height: 175px;
    }
}

/* <---------------media SCREEN -----------> */
@media screen and (min-width: 851px) and (max-width: 1050px) {
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

