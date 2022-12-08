<script>
    import photo from '/src/img/addinfo.svg'
    import Fa from 'svelte-fa'
    import {faTriangleExclamation, faHouse} from '@fortawesome/free-solid-svg-icons'

</script>

    <div class="background">
        <Fa icon={faTriangleExclamation}></Fa>This area is currently under construction. Come back soon! <Fa icon={faTriangleExclamation}></Fa>
    </div>
    <form action='/'><button class='home'><Fa icon={faHouse} size=2x></Fa><br>Home</button></form>
    <br>
    <br>
    <img class='pic' src={photo} alt="construction logo" >

    

<style>
.background {
    display: flex;
    width: 100%;
    height: 100%;
    text-align: center;
    font-size: 2rem;
    justify-content: center;
    margin-bottom: 30px;
}
.pic {
    width: 100%;
    height: 100%;
}
.home {
    display: block;
    width: 5rem;
    height: 5rem;
    margin: 0 auto;
    border: none;
    border-radius: 20%;
    background: var(--red);
    box-shadow: 0 8px #999;
    color: var(--white);
    font-size: large;
    text-decoration: none;    
}
.home:hover {
    cursor: pointer;
    background: #ff2e0eeb;
}
.home:active{
    transform: translateY(2px);
    box-shadow: 0 5px #666;
}

/* <---------------- PHONE/SMALL SCREEN ----------------> */

@media screen and (max-width: 800px) {
    .background {
        width: 100%;
    }
    .pic {
        position: relative;
    }
    .home {
    width: 4rem;
    height: 4rem;
    }
}
</style>