<script>
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin, faFacebook} from '@fortawesome/free-brands-svg-icons'
    import Burg from './Burg.svelte'


    export let first = {
        name: 'About Me',
        ref: '#about'
    }
    export let second = {
        name:'Services',
        ref: '#services'
    }

    export let third = {
        name:'Projects/Work',
        ref: '#projects'
    }

    export let fourth =  {
    name:'Contact Me', 
    ref: 'mailto:bpeif21@gmail.com'
    }
</script>
<nav href='#top'>
<div class="navbar">
    
    <div class="menu" >
        <li class="nav_item"><a href={first.ref} >{first.name}</li>
        <li class="nav_item"><a href={second.ref} >{second.name}</a></li>
        <li class="nav_item"><a href={third.ref} >{third.name}</a></li>
        <li class="nav_item"><a href={fourth.ref}>{fourth.name}</a></li>
            <div class="link_FA">
                <a href=https://github.com/brodiep21 rel="noreferrer" target="_blank"><Fa icon={faGithub} size=2.5x primaryColor= 'black'/></a>
                <a href=https://www.linkedin.com/in/brodie-peif-871164230 rel="noreferrer" target="_blank"><Fa icon={faLinkedin} size=2.5x primaryColor='black'/></a>
                <a href=https://www.facebook.com/bpeif rel="noreferrer" target="_blank"><Fa icon={faFacebook} size=2.5x primaryColor='black'/></a>
            </div>
        </div>
        
        <div class="burg">
            <Burg/>
        </div>
       
    <!-- <DropMenu /> -->
	
    </div>
</nav>
<style>
    nav {
    position: fixed;
    width: 100%;
    top: 0;
    left: 0;
    background-color: var(--white);
    z-index: 100;
    }

    /* <------------- SMALL SCREEN --------------> */
    @media screen and (max-width: 1159.9px){
    .navbar {
    border-bottom-color: var(--grey);
    border-bottom: 1px solid;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
    height: 60px;
    display: flex;
    position: relative;
    background-color: var(--white);
    
    }
    .menu {
        display: none;
    }
    .link_FA {
        display: none;
    }
}

    /* <------------- LARGE SCREEN --------------> */
@media screen and (min-width: 1160px) {
.navbar {
    color: var(--grey);
    border-bottom: 1px solid;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
    height: 65px;
    padding-left: 25px;
    padding-right: 25px;
    font-weight: 100;
}
.navbar a {
    position: relative;
    display: inline-block;
    font-size: 1.5em;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    background: linear-gradient(to right, var(--orange),var(--orange) 50%, rgb(0, 0, 0) 50%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-size: 200% 100%;
    background-position: 100%;
    transition: background-position 500ms ease;
}
.burg {
    display: none;
    }
.menu {
    display: flex;
    list-style: none;
    column-gap: 4em;
}

.nav_item {
    margin-top: .4em;
    font-size: 24px;
}
.navbar a:hover{
    background-position: 0 100%;
}

.link_FA {
    display: flex;
    margin-left: auto;
    column-gap: .5em;
}
.link_FA ::after {
    content: '';
    width: 100%;
    position: absolute;
    transform: scaleX(0);
    height: 3px;
    bottom: 0px;
    border-radius: 2px;
    left: 0;
    background-color: var(--red);
    transform-origin: center;
    transition: transform 0.5s ease-out
}

.link_FA :hover:after {
    transform: scaleX(1);
    transform-origin: center;
}

}
</style>