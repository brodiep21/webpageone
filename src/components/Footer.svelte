<script>
     import {faArrowUp} from '@fortawesome/free-solid-svg-icons'
	import Fa from 'svelte-fa/src/fa.svelte';
    import vc from '../img/vc.jpg'
</script>

<footer>
    <div class="contact">
        <div class="vailcoding"></div>
        <a href='#top' class="top_arrow">
            <button type="button" class="top" ><Fa icon={faArrowUp} size=2x primaryColor=#F5F5F5 />
            </button>
        </a>
    </div>
    
    
    <div class="vailcoder">Designed by
        <img class="emblem" src={vc} alt="vailcoding emblem"> 
    </div>
       
</footer>

<style>
    footer {
        display: grid;
        grid-template-columns: 1;
        grid-template-rows: 50% 50%;
        min-height: 250px;
        /* background: radial-gradient(circle,  var(--purple) 5%, var(--veridian) 99%); */
    }
    .contact {
        background-color: var(--grey);
        border-radius: 4px;
    }
    .top_arrow {
        margin-left: auto;
    }
    .top {
        border-radius: 20px;
        width: 50px;
        height: 50px;
        background-color: var(--purple);
        border: none;
        text-align: center;
        transition: .15s ease-in;
    }
    .top:hover {
        transform: scale(1.3);
        cursor: pointer;
    }
    .vailcoder {
        font-family: var(--playfair);
       margin-left:auto;
       padding-top: 1.2em;
       padding-right: 1em;
       font-weight:900;
        text-transform: uppercase;
    }
    .emblem {
        width: 40px;
        height:40px;
        position: relative;
    }
</style>