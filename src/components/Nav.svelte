<script>
    import Fa from 'svelte-fa/src/fa.svelte'
    import {faGithub, faLinkedin} from '@fortawesome/free-brands-svg-icons'
    // import {} from '@fortawesome/free-brands-svg-icons'
</script>
<nav class="navbar">
    <div class="nav_list">
        <ul >
            <li class="nav_item"><a href="#about" class="navlink" >About Me</li>
            <li class="nav_item"><a href="#aspirations" class="navlink" >Aspirations</a></li>
            <li class="nav_item"><a href="#services" class="navlink" >My Services</a></li>
            <li class="nav_item"><a href="#work" class="navlink" >My Projects/Work</a></li>
        </ul>
    </div>
    <div class="container">
        <a href=https://github.com/brodiep21 rel="noreferrer" target="_blank"><Fa icon={faGithub} size=3x primaryColor= 'black'/></a>
        <a href=https://www.linkedin.com/in/brodie-peif-871164230 rel="noreferrer" target="_blank"><Fa icon={faLinkedin} size=3x primaryColor='black'/></a>
    </div>
</nav>
<style>
nav {
    color: rgba(13, 2, 2, 0.136);
    border-bottom: 1px solid;
}
.container {
    text-align: right;
    padding: 1em;
}
.nav_item {
    color: black;
    text-align: start;
}
</style>