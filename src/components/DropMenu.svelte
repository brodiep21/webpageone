<script context="module">
    export let showMenu = {false};
    import {createEventDispatcher} from 'svelte'

    
</script>


{#if showMenu}
<div class="dropMenu">
    <li class="nav"><a href="#about" class="navlink" >About Me</li>
    <li class="nav"><a href="#aspirations" class="navlink" >Aspirations</a></li>
    <li class="nav"><a href="#services" class="navlink" >Services</a></li>
    <li class="nav"><a href="#work" class="navlink" >Projects/Work</a></li>
</div>
{/if}
<style>
     
    .dropMenu {
    padding: 0;
    top: 100%;
    width: 100%;
    list-style: none;
    position: absolute;
    font-weight: 800;
    font-size: larger;
    background-color: #ffffffda;
    text-align: center;
    z-index: 3;
    }

    .dropMenu li a {
        text-decoration: none;
        color:rgb(0, 0, 0);
        text-transform: uppercase;
        transition: .5sec;
    }
    .dropMenu li a:hover {
        color:#3E92CC
    }

    @media screen and (min-width: 1006px) {
   
}
</style>