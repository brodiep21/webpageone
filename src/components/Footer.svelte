<script>
     import {faArrowUp} from '@fortawesome/free-solid-svg-icons'
	import Fa from 'svelte-fa/src/fa.svelte';
	import { onMount} from 'svelte/internal';
    import vc from '../img/vc.jpg'
    import {faGithub, faLinkedin, faFacebook} from '@fortawesome/free-brands-svg-icons'

   let time = new Date();

    $: hours = time.getHours();
	$: minutes = time.getMinutes();
	$: seconds = time.getSeconds();

    onMount(() => {
        const interval = setInterval(() => {
            time = new Date()
        }, 1000);

        return () => {
            clearInterval(interval);
        };
    });
    $: color = 'black'
    function valueCheck (val) {
        if (val < 10) {
            return '0' + val
        } 
        else {
            return val
        }
    }
    function colorShift () {
        color = '#2EC4B6'
        return color
    }
</script>

<footer>
    <div class="fmain">
        <div class="contact_arrow">
            <a href='#top' class="top_arrow">
                <button type="button" class="top" ><Fa icon={faArrowUp} size=2x primaryColor=#F5F5F5 />
                </button>
            </a>
        </div>
        <div class="contact_info">
            <div class="contact">
                <h2 class='name'>BP.</h2>
                <h2>Let's Get Started</h2>
                <h3>Build 2022</h3></div>
            <div class="phone">
                <h2>1-970-685-8088</h2>
                <h3>
                    {#if (hours-12 >= 1 && hours-12 <= 9)}
                    {0}{hours - 12}:{valueCheck(minutes)}:{valueCheck(seconds)} PM
                    {:else if (hours-12 > 10)}
                    {hours-12}:{valueCheck(minutes)}:{valueCheck(seconds)} PM
                    {:else}
                    {hours}:{valueCheck(minutes)}:{valueCheck(seconds)} AM
                    {/if}
                        <br>Images from 
                        <a href=https://undraw.co/illustrations rel="noreferrer" target="_blank">undraw.co</a>
                </h3>
            </div>
            <div class="address">
                <h3>Cape Coral <br> Florida, 33993</h3>
            </div>
        </div>
    </div>
    
    

    <div class="emblem">
        <img class="logo" src={vc} alt="vailcoding emblem"> 
        <!-- <div class="intouch"> -->
            <a href=https://github.com/brodiep21 rel="noreferrer" target="_blank">
                <Fa icon={faGithub} size=2.5x primaryColor= 'black'/>
            </a>
            <a href=https://www.linkedin.com/in/brodie-peif-871164230 rel="noreferrer" target="_blank">
                <Fa icon={faLinkedin} size=2.5x primaryColor='black'/>
            </a>
            <a href=https://www.facebook.com/bpeif rel="noreferrer" target="_blank">
                <Fa icon={faFacebook} size=2.5x primaryColor='black' primaryOpacity={.2}/>
            </a>
        <!-- </div> -->
    </div>
       
</footer>

<style>
    footer {
        display: grid;
        grid-template-columns: 75% 25%;
        min-height: 200px;
    }
    .fmain {
        background-color: var(--red);
        color: var(--white);
    }
   .contact_arrow {
    text-align: right;
    margin-top: 1rem;
    margin-right: 1rem;
   }
    .contact_arrow button {
        border-radius: 20px;
        width: 50px;
        height: 50px;
        background-color: var(--orange);
        border: none;
        transition: .15s ease-in;
        position: relative;
    }
    .contact_info {
        display: grid;
        grid-template-columns: 33.3% 33.3% 33.4%;
        justify-content: center;
        text-align:center;
    }
    .name {
        margin-bottom: -1.5rem;
        font-size: 1.8rem;
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    }
    .contact h3 {
        font-size: 1.2rem;
        font-weight: 100;
        margin-top: -1.2rem;
    }
    .top:hover {
        transform: scale(1.3);
        cursor: pointer;
    }
    .emblem {
        background-color: var(--lorange);
        justify-content: space-around;  
        display: flex;
    }
    .emblem .logo{
        width: 40px;
        height:40px;
    }
    .phone {
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        font-style:italic;
    }
    .phone h2 {
        margin-top: 1.5rem;
    }
    .phone h3 {
        margin-top: -1rem;
        
    }
    .phone a {
        color: var(--white);
    }
    .address {
        padding-top: 1rem;
    }
/* <---------------PHONE SCREEN -----------> */
@media screen and (max-width: 800px) {
    footer {
        grid-template-columns: 100%;
        grid-template-rows: 2;
    }
    .emblem {
        background-color: var(--lorange)
    }
    .contact_arrow {
        text-align:center;
        margin-right: 0rem;
    }
}
</style>