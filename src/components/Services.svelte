<script>
    // import {fade} from 'svelte/transition'
    import devpic from '../img/devpic3.svg'
    import devpic2 from '../img/devpic.svg'

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
            <p>Your small business needs a website?  Lets get you on the map, I offer a variety of choices.</p>
            <a href=/Services >Explore</a>
        </div>
        <div class="picture">
            
            <div class="picture2"><img src={devpic} alt="illustration of developer"></div>
        </div>
        <div class="picture3"><img src={devpic2} alt="illustration of developer"></div>
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
    min-height:30rem;
    color: var(--black);
}
.services1 {
    margin-top: 3rem;
}

.services1 h1 {
    font-size: 4rem;
    margin-left: 5rem;
    margin-bottom: 1.2rem;
    margin-top: .9rem;
}
.services h3 {
    margin-left: 5rem;
    margin-top: 2rem;
    font-family:'Courier New', Courier, monospace;
    font-size: larger;
}
.services1 p {
    margin-left: 5rem;
    margin-top: 3rem;
    margin-bottom: 2rem;
    font-size:larger;
}
.services1 a {
    margin-top: 5rem;
    margin-left: 5rem;
    font-size: 1.4rem;
    text-underline-offset: .6rem;
    transition: .3s ease-in-out;
    color: var(--black);
}
.services1 a:hover {
    color: var(--red)
}
.services2 {
    width: 40%;
    background-color: var(--red);
}
.picture {
    width: 70%;
    margin-left: auto;
    /* overflow: hidden; */
}
.picture2 {
    width: 40%;
    margin-left: 40%;
    padding-top: 1.6rem;
    
    overflow:visible;
}
.picture img{
    background-color: var(--white);
    border-radius: 5rem;
    box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.26);
    height: 375px;
    background-size: cover;
    background-repeat: no-repeat;
    transition: .3s ease-in-out;
    position:absolute;
    z-index: 1;
    margin-top: 1rem;;
    
}
.picture3 {
    display: none;
}

/* .picture:hover + .background{
    background-color: var(--black);
    width: 100px;
} */

/* <-----------------SMALL SCREEN-------------> */
@media screen and (min-width: 650px) and (max-width: 1110px) {
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
        margin-left: 20px;
    }
    .picture img {
        height: 200px;
    }
}

/* <---------------MEDIUM SCREEN -----------> */
@media screen and (min-width: 1111px) and (max-width: 1313px) {
    .picture {
        /* text-align: left; */
        padding-top: 1.6rem;
    }
    .picture2 {
        margin-left: 40%;
        padding-top: 2rem;
    }
    .picture img {
        height: 275px;
    }
}
/* <---------------PHONE SCREEN -----------> */
@media screen and (max-width: 649px) {
    .services1 {
        margin-left: -4rem;
        margin-top: 3rem;
    }
    .picture2 {
        margin-left: 0;
    }
    .picture img {
        display: none;
    }
    .picture3 {
        display: flex;
    }
    .picture3 img {
        width: 100px;
        height: 200px;
        position: relative;
        margin-left: -8em;
        margin-top: 2rem;
    }
}
</style>

