<script>
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin} from '@fortawesome/free-brands-svg-icons'
    // import {} from '@fortawesome/free-brands-svg-icons'
</script>
<nav class="navbar">
    <div class="hamburg">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
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
    <!-- <div class="container">
        
        
    </div> -->
</nav>
<style>
nav {
    color: rgba(13, 2, 2, 0.136);
    border-bottom: 1px solid;
}
.nav_list {
    color: black;
    text-align: start;
    display: flex;
    text-decoration: none;
    font-size: 18px;
    list-style: none;
    height: 100%;
    width: 95%;
    justify-content:left;
    column-gap: 5px;
}

.link_FA {
    display: flex;
    margin-left: auto;
    column-gap: 10px
}
@media screen and (max-width: 768px){
    .line {
        width: 30px;
        height: 5px;
        background:black;
        margin: 5px;
    }
    .nav_list{
        position: fixed;
        height: 100vh;
        width: 100%;
        flex-direction:column;
        display: none;
    }
}
</style>