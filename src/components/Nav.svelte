<script>
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin, faFacebook} from '@fortawesome/free-brands-svg-icons'
    // import {} from '@fortawesome/free-brands-svg-icons'

    
</script>
<nav>
    <div class="hamburg">
        <input type="checkbox">
        <!-- <div id="line" class="line"></div>
        <div id="line" class="line"></div>
        <div id="line" class="line"></div> -->
        <span></span>
        <span></span>
        <span></span>
        <div class="menu">
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
    </div>
</nav>

<style>

    /* <------------- SMALL SCREEN --------------> */
    @media screen and (max-width: 1005px){
     nav {
    color: rgb(68, 65, 65);
    border-bottom: 1px solid;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
    height: 60px;
    content-visibility: hamburg;
    }

    .hamburg {
        padding: 15px;
        position: relative;
        /* display: flex; */
        width: 40px;
        height: 22px;
        border-radius: 20px;
        box-shadow: 0 1px 4px black;
        background-color: #ffffff;
        transition: .5sec;
        justify-content: center;
        margin-left: 45%;
        overflow: hidden;
    }

    .hamburg input {
        width: 30px;
        height: 21px;
        margin-top: 0;
        opacity: 0;
        cursor:pointer;
        position: absolute;
    }
    .hamburg input:checked ~ .menu {
        width: 500px;
    }

    .menu {
        margin: 0;
        padding: 0;
        width: 0;
        overflow: hidden;
        transition: .5sec;
    }
    .menu li {
        list-style: none;
        margin: 0 10px;
    }
    .menu li a {
        text-decoration: none;
        color:black;
        text-transform: uppercase;
        font-weight: 800;
        transition: .5sec;
    }
    .menu li a:hover {
        color:#3E92CC
    }
    .hamburg span {
        position:absolute;
        width: 30px;
        height: 4px;
        margin-top: 9px;
        margin-left: 4px;
        border-radius: 50px;
        background-color: black;
        pointer-events: none;
        transition: .5sec;
    }
    .hamburg span:nth-child(2) {
        transform: translateY(-8px)
    }
    .hamburg span:nth-child(3) {
        transform: translateY(8px)
    }
    /* .hamburg span :hover {
        background-color: white;
    } */
    .hamburg input:checked ~ span {
        background-color: rgb(233, 68, 68);
    }
    .hamburg input:checked ~ span:nth-child(2) {
        transform: translateY(0) rotate(-45deg);
    }
    .hamburg input:checked ~ span:nth-child(3) {
        transform: translateY(0) rotate(45deg);
    }
    .hamburg input:checked ~ span:nth-child(4) {
        display:none;
    }

    .link_FA {
        display: none;
    }
}

    /* <------------- LARGE SCREEN --------------> */
@media screen and (min-width: 1006px) {
nav {
    color: rgb(68, 65, 65);
    border-bottom: 1px solid;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
    height: 60px;
}
nav a {
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
.menu {
    display: flex;
    list-style: none;
    column-gap: 2em;
    justify-content: space-evenly;
}

.nav_item {
    margin-top: .4em;
    font-size: 24px;
}
nav a:hover{
    background-position: 0 100%;
}
.hamburg input {
  display: none;
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