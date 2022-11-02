<script>
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin} from '@fortawesome/free-brands-svg-icons'
    // import {} from '@fortawesome/free-brands-svg-icons'

    // function colorshift() {
    //   var div = document.getElementById("line")
    //  if (div.style.background= "black") {
    //     div.style.background = "red";
    //  } else {
    //     div.style.background= "black"
    //  }
    // on:mouseover={colorshift} on:mouseout={colorshift} on:focus={colorshift} on:blur={colorshift}
    // }
</script>
<nav class="navbar">
    <div class="hamburg" >
        <div id="line" class="line"></div>
        <div id="line" class="line"></div>
        <div id="line" class="line"></div>
        <ul class="nav_list">
            <li class="nav_item"><a href="#about" class="navlink" >About Me</li>
            <li class="nav_item"><a href="#aspirations" class="navlink" >Aspirations</a></li>
            <li class="nav_item"><a href="#services" class="navlink" >My Services</a></li>
            <li class="nav_item"><a href="#work" class="navlink" >My Projects/Work</a></li>
        <div class="link_FA">
            <a href=https://github.com/brodiep21 rel="noreferrer" target="_blank"><Fa icon={faGithub} size=2.5x primaryColor= 'black'/></a>
            <a href=https://www.linkedin.com/in/brodie-peif-871164230 rel="noreferrer" target="_blank"><Fa icon={faLinkedin} size=2.5x primaryColor='black'/></a>
        </div>
        </ul>
        <!-- <div class="box"></div> -->
    <!-- <div class="container">
        
        
    </div> -->
</nav>
<style>
nav {
    color: rgb(68, 65, 65);
    border-bottom: 1px solid;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
    height: 55px;
}

.nav_list {
    color: black;
    text-align:center;
    display: flex;
    text-decoration: none;
    font-size: 19px;
    list-style: none;
    height: 100%;
    width: 95%;
    column-gap: 5px;
}

.link_FA {
    display: flex;
    margin-left: auto;
    column-gap: 12px;
}
.link_FA :hover {
    box-shadow: 0 1px 0 rgb(89, 86, 86);
    /* transform: box-shadow .3s ease-in-out; */
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
@media screen and (max-width: 768px){
    nav {
    color: rgb(68, 65, 65);
    border-bottom: 1px solid;
    height: 55px;
    box-shadow: 0 1px 0 rgba(0, 0, 0, 0.336);
}

    .line {
        width: 30px;
        height: 5px;
        background:black;
        margin: 5px;
    }
    .hamburg {
        cursor:pointer;
        width: 40px;
        position: absolute;
    }
    .link_FA {
    /* width: 10%; */
    margin-left: auto;
    column-gap: 12px;

    }
    /* .navlink {
        position: fixed;
        height: 100vh;
        width:100%;
        flex-direction:column;
        clip-path: circle(100px at 90% -10%);
        -webkit-clip-path: circle(100px at 90% -10%);
        transition: all 1s ease-out;
    }
    .navlink.open {
        clip-path: circle(100px at 90% -10%);
        -webkit-clip-path: circle(100px at 90% -10%);

    } */
    .nav_list{
        position: fixed;
        height: 100vh;
        width: 100%;
        flex-direction:column;
        display: none;
    }
}
</style>