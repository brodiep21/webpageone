<script>
    
	import Burg, {openMenu} from '../components/Burg.svelte'
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin, faFacebook} from '@fortawesome/free-brands-svg-icons'

</script>
<div class="navbar">
    <div class="menu" {openMenu}>
        <li class="nav_item"><a href="#about" class="navlink" >About Me</li>
        <li class="nav_item"><a href="#aspirations" class="navlink" >Aspirations</a></li>
        <li class="nav_item"><a href="#services" class="navlink" >Services</a></li>
        <li class="nav_item"><a href="#work" class="navlink" >Projects/Work</a></li>
            <div class="link_FA">
                <a href=https://github.com/brodiep21 rel="noreferrer" target="_blank"><Fa icon={faGithub} size=2.5x primaryColor= 'black'/></a>
                <a href=https://www.linkedin.com/in/brodie-peif-871164230 rel="noreferrer" target="_blank"><Fa icon={faLinkedin} size=2.5x primaryColor='black'/></a>
                <a href=https://www.facebook.com/bpeif rel="noreferrer" target="_blank"><Fa icon={faFacebook} size=2.5x primaryColor='black'/></a>
            </div>
        </div>
       <div class="burg"><Burg/></div>
    <!-- </div> -->
    </div>

<style>


    /* <------------- SMALL SCREEN --------------> */
    @media screen and (max-width: 1005px){
    .navbar {
    border-bottom-color: rgb(68, 65, 65);;
    border-bottom: 1px solid;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
    height: 60px;
    display: flex;
    position: relative;
    }
    .burg {
        padding-left: 1.5em;
        padding-top: .7em;
        position:absolute;
        z-index: 3;
    }
    .menu {
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

    .menu li a {
        text-decoration: none;
        color:rgb(0, 0, 0);
        text-transform: uppercase;
        transition: .5sec;
    }
    .menu li a:hover {
        color:#3E92CC
    }

    .link_FA {
        display: none;
    }
}

    /* <------------- LARGE SCREEN --------------> */
@media screen and (min-width: 1006px) {
.navbar {
    color: rgb(68, 65, 65);
    border-bottom: 1px solid;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
    height: 60px;
    display: fit-content;
}
.navbar a {
    position: relative;
    display: inline-block;
    font-size: 1.4em;
    font-weight: 800;
    overflow: hidden;
    background: linear-gradient(to right, #3E92CC, #3E92CC 50%, rgb(0, 0, 0) 50%);
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
    column-gap: 2em;
    justify-content: fit-content;
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
    height: 2px;
    bottom: 0px;
    left: 0;
    background-color: #3E92CC;
    transform-origin: center;
    transition: transform 0.3s ease-out;
}

.link_FA :hover:after {
    transform: scaleX(1);
    transform-origin: center;
}
/* .box {
  position: relative;
  display: inline-block;
  width: 100px;
  height: 100px;
  background-color: #fff;
  border-radius: 5px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
  border-radius: 5px;
  -webkit-transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
  transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
}

.box::after {
  content: "";
  border-radius: 5px;
  position: absolute;
  z-index: -1;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
  opacity: 0;
  -webkit-transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
  transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
}

.box:hover {
  -webkit-transform: scale(1.25, 1.25);
  transform: scale(1.25, 1.25);
}

.box:hover::after {
    opacity: 1;
} */
}
</style>