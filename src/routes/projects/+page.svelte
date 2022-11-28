<script>
    import photo from '/src/img/addinfo.svg'
    import Fa from 'svelte-fa'
    import {faTriangleExclamation, faHouse} from '@fortawesome/free-solid-svg-icons'

</script>
    <div class="background">
        <Fa icon={faTriangleExclamation}></Fa>This area is currently under programming construction. Come back soon! <Fa icon={faTriangleExclamation}></Fa>
        
    </div>
    <img class='pic' src={photo} alt="construction logo" >

    <button class='home'><a href='/'><Fa icon={faHouse}></Fa><br>Home</a></button>
<style>
.background {
    display: flex;
    width: 100%;
    height: 100%;
    text-align: center;
    font-size: 2rem;
    justify-content: center;
    margin-bottom: 100px;
}
.pic {
    width: 100%;
    height: 100%;
}
.home {
    display: block;
    margin: 0 auto;
}

/* <---------------- PHONE/SMALL SCREEN ----------------> */

@media screen and (max-width: 800px) {
    .background {
        width: 100%;
    }
    .pic {
        position: relative;
    }
}
</style>