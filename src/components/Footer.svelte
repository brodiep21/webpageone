<script>
     import {faArrowUp} from '@fortawesome/free-solid-svg-icons'
	import Fa from 'svelte-fa/src/fa.svelte';
    import vc from '../img/vc.jpg'
</script>

<footer>
    <a href='#top' class="top_arrow">
        <button type="button" class="top" ><Fa icon={faArrowUp} size=2x primaryColor=#F5F5F5 />
        </button>
        
    </a>
    
    <div class="vailcoder">Designed by
        <img class="emblem" src={vc} alt="vailcoding emblem"> 
    </div>
       
</footer>

<style>
    footer {
        display: grid;
        grid-template-columns: 55% 45%;
        /* background: radial-gradient(circle,  var(--purple) 5%, var(--veridian) 99%); */
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
       margin-left:auto;
       padding-top: 1.2em;
       padding-right: 1em;
       font-weight:100;
       font-style: oblique;
       font-size: larger;
    }
    .emblem {
        width: 40px;
        height:40px;
        position: absolute;
    }
</style>