<script>
     import {faArrowUp} from '@fortawesome/free-solid-svg-icons'
	import Fa from 'svelte-fa/src/fa.svelte';
    import vc from '../img/vc.jpg'
</script>

<footer>
    <div class="contact">
        <a href='#top' class="top_arrow">
            <button type="button" class="top" ><Fa icon={faArrowUp} size=2x primaryColor=#F5F5F5 />
            </button>
        </a>
    </div>
    
    

    <div class="emblem">
        <img class="emblem" src={vc} alt="vailcoding emblem"> 
    </div>
       
</footer>

<style>
    footer {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        min-height: 150px;
    }
    .contact {
        background-color: var(--red);
    }
    .top_arrow {
        margin-left: auto;
    }
    .contact button {
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
    .emblem {
        padding-top: 1rem;
        width: 40px;
        height:40px;
    }
</style>