<script >
    import {fly} from 'svelte/transition';
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin, faFacebook} from '@fortawesome/free-brands-svg-icons'
    $: showMenu = false;

    // function animate (node, options) {
    //     if (showMenu) {
    //         return options.fn(node, options);
    //     }
    // }
    // in:animate={{fn: slide, duration:750, y:500}} out:animate={{fn: slide, duration:500, y:500}}
</script>

    <label for="check">
            <input type="checkbox" id="check" on:click={() => showMenu = !showMenu} /> 
            <span></span>
            <span></span>
            <span></span>
    </label>
    {#if showMenu}
    <div class="dropMenu" transition:fly="{{y: -100, duration: 1000}}">
        <li class="nav"><a href="#about" class="navlink" >About Me</li>
        <li class="nav"><a href="#aspirations" class="navlink" >Aspirations</a></li>
        <li class="nav"><a href="#services" class="navlink" >Services</a></li>
        <li class="nav"><a href="#work" class="navlink" >Projects/Work</a></li>
        <div class="icons"><a href=https://github.com/brodiep21 rel="noreferrer" target="_blank"><Fa icon={faGithub} size=2.5x primaryColor= 'black'/></a>
        <a href=https://www.linkedin.com/in/brodie-peif-871164230 rel="noreferrer" target="_blank"><Fa icon={faLinkedin} size=2.5x primaryColor='black'/></a>
        <a href=https://www.facebook.com/bpeif rel="noreferrer" target="_blank"><Fa icon={faFacebook} size=2.5x primaryColor='black'/></a>
      </div>
    </div>
    
    {/if}
<style>

label{
  display:flex;
  flex-direction:column;
  width:50px;
  cursor:pointer;
  position: absolute;
  margin-left: 5px;
  margin-top: .7em;
}

label span{
  background: #000000;
  border-radius:10px;
  height: 5px;
  margin: 3px 0;
  transition: .7s  cubic-bezier(0.68, -0.6, 0.32, 1.6);
}

span:nth-of-type(1){
  width:100%;
  
}

span:nth-of-type(2){
  width:100%;
}


span:nth-of-type(3){
  width:100%;
 
}


input[type="checkbox"]{
  display:none;
}


input[type="checkbox"]:checked ~ span:nth-of-type(1){
  transform-origin:bottom;
  width: 50%;
  background-color: rgb(255, 20, 20);
  transform:rotatez(45deg) translate(3px,-2px)
}


input[type="checkbox"]:checked ~ span:nth-of-type(2){
  
  transform-origin:top;
  width: 100%;
  background-color: rgb(255, 20, 20);
  transform:rotatez(-45deg)
}


input[type="checkbox"]:checked ~ span:nth-of-type(3){
  
  transform-origin:bottom;
  width:50%;
  background-color: rgb(255, 20, 20);
  transform: translate(21px,-4px) rotatez(45deg);

}
.dropMenu {
    padding: 0;
    top: 100%;
    width: 100%;
    list-style: none;
    position: absolute;
    font-weight: 800;
    font-size: 26px;
    background-color: #ffffffce;
    z-index: 3;
    text-align: center;
    box-shadow:0px 1px#000000 
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
    .nav {
      margin-bottom: 10px
    }
    .icons {
      display: flex;
      justify-content: space-around;
    }
</style>