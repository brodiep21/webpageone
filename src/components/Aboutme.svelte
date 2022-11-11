<script>
    import Profilepic from '../img/profilepic.jpg'
    import Image from '../img/s.png'
</script>
<section class="about_me" href=#about>
    
    <div class="whitespace">
        <div class="rectangle">
            <h1 class="about_me_title">Hi, I'm Brodie Peif</h1>
        </div>
    </div>
    <div class="outer_rect">
        
        <img class="profile_pic" src={Profilepic} alt="Brodie smiling">
    </div>
    
    
</section>
<div class="anecdote"><h1>Full time employee by day, Crossfit coach in the afternoon, dedicated programmer by night</h1></div>
<!-- <div class="box"></div> 
<div class="box"></div><div class="box"></div><div class="box"></div><div class="box"></div><div class="box"></div> -->

<style>
.anecdote {
    width: 95%;
    text-align: center;
}
/* .box {
  position: relative;
  display: inline-block;
  width: 200px;
  height: 200px;
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
.profile_pic {
    border-radius: 20%;
    width: 225px;
    height: 250px;
    box-shadow: 0px 6px 15px  grey;
    position: relative;
    margin-right: 25%;
}
/* .profile_pic:hover {
    box-shadow: 0px 6px 15px grey;
    transform:scale(1.3);
    z-index: 3;
} */
.about_me {
    width: 100%;
    height: 300px;
    margin-top:100px;
    display: grid;
    z-index: -100;
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
  background-color: var(--veridian);
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 5px rgb(119, 117, 117);
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
   margin-top: 15px;
   text-align: justify;
   width:100% inherit;
   margin-left: 60% ;
   text-shadow: 0px 1px 1px rgba(44, 44, 44, 0.341);
   font-family: sans-serif;
   color: rgba(0, 0, 0, 0.652);
   font-size: 26px;
   z-index: -100;
}


/* <---------------- PHONE SCREEN ----------------> */
@media screen and (max-width: 450px) {
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
  background-color: #3E92CC;
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 5px rgb(119, 117, 117);
  text-align: center;
}
.about_me {
    width: 100%;
    height: 200px;
    margin-top:80px;
    display: flex;
}
h1.about_me_title {
   justify-content:right;
   margin-top: 11px;
   text-align: justify;
   width:100% inherit;
   margin-left: 48% ;
   text-shadow: 0px 1px 1px rgba(44, 44, 44, 0.126);
   font-family: sans-serif;
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
  background-color: #3E92CC;
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 5px rgb(119, 117, 117);
  text-align: center;
}
.about_me {
    width: 100%;
    height: 250px;
    margin-top:80px;
    display: flex;
}
h1.about_me_title {
   justify-content:right;
   margin-top: 15px;
   text-align: justify;
   width:100% inherit;
   margin-left: 50% ;
   text-shadow: 0px 1px 1px rgba(44, 44, 44, 0.126);
   font-family: sans-serif;
   color: rgba(0, 0, 0, 0.652);
   font-size: 24px;
}
.profile_pic {
    border-radius: 20%;
    width: 150px;
    height: 175px;
    box-shadow: 0px 6px 15px  grey;
    position: relative;
    margin-right: 65%;
}
}
</style>