<script>
	import Fa from 'svelte-fa/src/fa.svelte'

    import Profilepic from '../img/profilepic.jpg'
    import background from '../img/hellot.png'
    import {faFileLines, faAngleRight} from '@fortawesome/free-solid-svg-icons'
</script>
<section class="about_me" href='#about' id='about'>
    
    <div class="whitespace">
        <div class="rectangle">
            <h1 class="about_me_title">Hi, I'm Brodie Peif</h1>
        </div>
    </div>
    <div class="outer_rect">
        
        <img class="profile_pic" src={Profilepic} alt="Brodie smiling">
    </div>
    
    
</section>
<div class="hello">
    <div class="box"></div> 
<div class="anecdote">
   <img class="hello" src={background} alt="hello text">
   
    <h1 class= "metitle">About Me.</h1>
    
    <h2 class="me1">Aspiring full-time developer, I design websites for small companies and work on backend developer projects with mentors from bluemodus and greymatter.</h2>
    <div class="learnmore"><a href="/aboutme">Learn More</a></div>
    <div class="doc"><button on:click={ () => window.open('https://docs.google.com/document/d/1q8Du_bYL3ckKOHOhYog7Qqp3MvruETFn/edit?usp=sharing&ouid=116822994425715327585&rtpof=true&sd=true')}> View My Resume</button></div>
    <!-- <div class="quote">
       <h2>"Don't focus on what you think you deserve, take aim at what you are willing to earn"</h2><h2 style="text-align: right">- David Goggins</h2></div> -->
       

</div>
</div>

<style>
.about_me {
    width: 100%;
    height: 300px;
    padding-top:100px;
    display: grid;
    z-index: -100;
}
.hello img{
    height: 40rem;
    width: 200%;
    image-resolution: auto;
    padding-left: 20rem;
}
.anecdote {
    max-height: 500px;
    display: grid;
    grid-template-columns: 33% 33% 33%;
    grid-template-rows: 30% 30% 30%;
    background: var(--teal);
    overflow: hidden;
}
.metitle{
    font-size: 3rem;
    grid-column-start: 2;
}
.me1 {
    padding-left: 3rem;
    align-self: center;
    grid-column-start: 2;
    grid-column-end: 4;
    grid-row-start: 2;
    grid-row-end: 3;
    color: var(--black);
}
.learnmore {
    grid-column-start: 2;
    grid-row-start: 3;
    padding-top: 8rem;
    padding-left: 1rem;
    
}
.learnmore a {
    color: var(--white);
    font-size: 1.4rem;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    text-underline-offset: .6rem;
    transition: .5s ease-in-out;
}
.learnmore :hover {
    color: var(--black);
}
 /* .learnmore a:after {
    position:absolute;
    width: 100%;
    transform: scaleX()
 } */
/* .quote {
    padding-top: 1rem;
    text-align: left;
    color:var(--black);
    padding-left: 8px;
    font-weight: 100;
    grid-column-start: 3;
    grid-column-end: 4;
    grid-row-start: 3;

} */

/* .box {
  position: relative;
  width: 250px;
  height: 400px;
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
  z-index: 1000;
}

.box:hover::after {
    opacity: 1;
} */
.profile_pic {
    border-radius: 20%;
    width: 225px;
    height: 250px;
    box-shadow: 0px 6px 15px  grey;
    position: relative;
    margin-right: 25%;
}

.whitespace {
    position: absolute;
    height: 100px;
    width: 75%;
    margin-top: 40px;
    display: flex;
    justify-content: center;
    z-index: -100;
}
.rectangle {
  height: 55px;
  width: 75%;
  max-width: 800px;
  background-color: var(--orange);
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 5px var(--grey);
  text-align: center;
  z-index: -100;
}
.about_me {
  display: flex;
  justify-content: center;
  z-index: -100;
}
.about_me_title {
    position:absolute;
    display:flex;
    z-index: -100;
}
.outer_rect {
    width: 75%;
    display: flex;
    justify-content: center;
    z-index: -100;
}

h1.about_me_title {
   justify-content:right;
   margin-top: 13px;
   text-align: justify;
   width:100% inherit;
   margin-left: 60% ;
   text-shadow: 0px 1px 1px rgba(44, 44, 44, 0.341);
   color: rgba(0, 0, 0, 0.652);
   font-size: 26px;
   z-index: -100;
   font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
   font-style: oblique;
   font-weight: 100;
}

.doc {
    grid-column-start: 3;
    grid-row-start: 3;
    padding-top: 7.3rem;
}
.doc button {
    background-color: #f5f5f50e;
    border-radius:30px;
    color: var(--white);
    border-color: var(--white);
    border: 2px solid var(--white);
    font-size: 1.4rem;
    font-weight:700;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    width: 15rem;
    height: 3rem;
    transition: .5s ease-in-out;
}
.doc button:hover {
    cursor: pointer;
    background-color: var(--black);
    border: 2px solid var(--black);
}
/* <---------------- PHONE SCREEN ----------------> */
@media screen and (max-width: 450px) {
    .hello img{
    height: 20rem;
    width: 300%;
    image-resolution: auto;
    padding-left: 2rem;
    padding-top: 15rem;
}
    .whitespace {
    position: absolute;
    height: 100px;
    width: 100%;
    margin-top: 30px;
    display: flex;
}
.rectangle {
  height: 45px;
  width: 75%;
  min-width: 375px;
  background-color: var(--orange);
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 5px var(--grey);
  text-align: center;
}
.about_me {
    width: 100%;
    height: 200px;
    padding-top: 80px;
    display: flex;
}
h1.about_me_title {
   justify-content:right;
   margin-top: 11px;
   text-align: justify;
   width:100% inherit;
   margin-left: 48% ;
   text-shadow: 0px 1px 1px rgba(44, 44, 44, 0.126);
   font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
   color: rgba(0, 0, 0, 0.652);
   font-size: 22px;
}
.profile_pic {
    border-radius: 20%;
    width: 150px;
    height: 175px;
    box-shadow: 0px 6px 15px  grey;
    position: relative;
    margin-right: 65%;
}
.anecdote {
    text-align: left;
    background: var(--teal);
}
.anecdote h1 {
    grid-column-end: 4;
}
.me1 {
    padding-top: 5rem;
    align-self: center;
    grid-column-start: 1;
    grid-column-end: 4;
    grid-row-start: 2;
    grid-row-end: 3;
    color: var(--black);
}
.learnmore {
    grid-column-start: 1;
    grid-column-end: 4;
}

}
/* <---------------- SMALL SCREEN ----------------> */
@media screen and (min-width: 451px) and (max-width: 1000px){
    .whitespace {
    position: absolute;
    height: 100px;
    width: 100%;
    margin-top: 30px;
    display: flex;
}
.rectangle {
  height: 55px;
  width: 70%;
  min-width: 350px;
  background-color: var(--orange);
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 5px var(--grey);
  text-align: center;
}
.about_me {
    width: 100%;
    height: 250px;
    padding-top: 80px;
    display: flex;
}
h1.about_me_title {
   justify-content:right;
   margin-top: 13px;
   text-align: justify;
   width:100% inherit;
   margin-left: 50% ;
   text-shadow: 0px 1px 1px rgba(44, 44, 44, 0.126);
   font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
   color: rgba(0, 0, 0, 0.652);
   font-size: 28px;
}
.profile_pic {
    border-radius: 20%;
    width: 150px;
    height: 175px;
    box-shadow: 0px 6px 15px  var(--grey);
    position: relative;
    margin-right: 65%;
}
.metitle {
    grid-column-end: 4;
}
}
</style>