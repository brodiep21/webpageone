<script>
     import {faArrowUp} from '@fortawesome/free-solid-svg-icons'
	import Fa from 'svelte-fa/src/fa.svelte';
    import vc from '../img/vc.jpg'
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
                <h3>© 2022</h3></div>
            <div class="phone">
                <h2>1-970-685-8088</h2>
            </div>
        </div>
        
    </div>
    
    

    <div class="emblem">
        <img class="logo" src={vc} alt="vailcoding emblem"> 
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
        padding-left: 1rem;
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
        grid-template-columns: 30% 30% 30%;
        /* grid-template */
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
    .emblem .logo{
        width: 40px;
        height:40px;
    }
    .phone {
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        font-style:italic;
    }
</style>