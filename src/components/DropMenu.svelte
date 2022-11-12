<script module='context'>
    import {fly} from 'svelte/transition';
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin, faFacebook} from '@fortawesome/free-brands-svg-icons'

    // export let showMenu = false;
</script>

<div class="dropMenu" transition:fly="{{y: -100, duration: 1000}}">
    <li class="nav"><a href="#about" class="navlink" >About Me</li>
    <li class="nav"><a href="#aspirations" class="navlink" >Services</a></li>
    <li class="nav"><a href="#services" class="navlink" >Projects/Work</a></li>
    <li class="nav"><a href="#contact" class="navlink" >Contact Me</a></li>
        <div class="icons">
            <a href=https://github.com/brodiep21 rel="noreferrer" target="_blank"><Fa icon={faGithub} size=2.5x primaryColor= 'black'/></a>
            <a href=https://www.linkedin.com/in/brodie-peif-871164230 rel="noreferrer" target="_blank"><Fa icon={faLinkedin} size=2.5x primaryColor='black'/></a>
            <a href=https://www.facebook.com/bpeif rel="noreferrer" target="_blank"><Fa icon={faFacebook} size=2.5x primaryColor='black'/></a>
        </div>
</div>


<style>
.dropMenu {
    padding: 0;
    top: 100%;
    width: 100%;
    list-style: none;
    position: absolute;
    font-weight: 100;
    font-size: 26px;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    background-color: #f5f5f5d0;
    z-index: 3;
    text-align: center;
    box-shadow:0px 1px var(--black) ;
    }
.nav {
    margin-bottom: 1px;
    /* display: inline-block; */
}
.dropMenu li a {
    text-decoration: none;
    color:rgb(0, 0, 0);
    text-transform: uppercase;
    transition: .5sec;
}
.dropMenu li a:hover {
    color:var(--purple)
}
.icons {
    display: flex;
    justify-content: space-around;
}
@media screen and (min-width: 741px) {

.nav {
    display: inline-block;
    padding: 1em;
}
}
@media screen and (max-width: 740px) {
    .nav {
        padding-bottom: 15px;
    }
}
</style>