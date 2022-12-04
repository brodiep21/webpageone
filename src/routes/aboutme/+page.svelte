<script>
    import Nav from "/src/components/Nav.svelte"
    import Fa from 'svelte-fa'
    import {faHouse} from '@fortawesome/free-solid-svg-icons'

    let first ={
        name:'Home',
        ref: '/'
    }
    let second = {
        name: 'Services',
        ref: '/#services'
    }
    let vidauto = true
</script>
<div class="filler"></div>
<div class="aboutme">
    <div class="initials">BP.</div>
    <h2>Brodie Peif</h2>
    <h1>About me.</h1>
</div>
<!-- <div class='background'> -->
    <Nav first={first} second={second}/>
    <div class="intro">
        <div class="vidtext">I love Crossfit, it's become a passion of mine. A healthy body promotes a healthy mind.</div>
        <div class="vid1 video">  
            <video src='/src/img/crossfitworkout.mp4' autoplay={vidauto} loop={vidauto} muted={vidauto}> <track kind='captions'></video>
        </div>
        <div class="vid2 video">
            <video src='/src/img/crossfitworkout3.mp4' autoplay={vidauto} loop={vidauto} muted={vidauto}> <track kind='captions'></video>
        </div>
        <div class="vid3 video">
            <video src='/src/img/crossfitworkout2.mp4' autoplay={vidauto} loop={vidauto} muted={vidauto}> <track kind='captions'></video>
        </div>
    </div>
<!-- </div> -->

<div class="pictures">
    <img src='/src/img/fishing.jpg' alt="brodie holding a fish">
</div>

<style>
@import url('https://fonts.cdnfonts.com/css/montserrat');
@import url('https://fonts.cdnfonts.com/css/playfair-display');
.filler {
    padding-top:80px;
}
.initials {
    padding-top:1rem;
    margin-left: 95%;
    font-size: 2.5rem;
    font-weight: 700;
    letter-spacing:-2px;
    font-family: 'Montserrat';
}
.aboutme {
    text-align:center;
    background: var(--orange);
    min-height: 200px;
}
.aboutme h2 {
    margin-top: 0;
    padding-top: 3rem;
    font-size: 2rem;
    font-family: 'Montserrat';
    margin-bottom: 0;
}
.aboutme h1 {
    margin-bottom: 0;
    margin-top: 0;
    padding-bottom: 4rem;
    font-size: 4rem;
    font-family: 'Montserrat';
    font-weight: 800;
}
.intro {
    display: grid;
    grid-template-columns: 33%, 33%, 33%;
    grid-template-rows: 10% 90%;
    text-align: center;
    background: url('/src/img/background2.png');
    background-size: cover;
}
.vidtext {
    color: var(--white);
    font-size: 2.5rem;
    width: auto;
    text-align: center;
    grid-column-start: 1;
    grid-column-end: 4;
    padding-top: 20px;
}
.vid1 {
    grid-column-start: 1;
}
.vid2 {
    grid-column-start: 2;
    
}
.vid3 {
    grid-column-start: 3;
}

.video video{
    max-height:1080px;
}
.pictures img {
    max-height: 700px;
    /* position: relative; */
}
/* <---------------- PHONE/SMALL SCREEN ----------------> */

@media screen and (max-width: 800px) {
.initials { 
 margin-left: 80%   
}
.intro {
    display: inline-block;
}
.video video {
    width:100%
}
.vidtext{
    color: var(--black)
}
.pictures img {
    width: 100%;
}
}
</style>