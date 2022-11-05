<script>
    import Profilepic from '../img/profilepic.jpg'
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
    

<style>
.profile_pic {
    border-radius: 20%;
    width: 225px;
    height: 250px;
    box-shadow: 0px 6px 15px  grey;
    position: relative;
    margin-right: 25%
}
.about_me {
    width: 100%;
    height: 300px;
    margin-top:15px;
    display: flex;
}
.whitespace {
    position: absolute;
    height: 100px;
    width: 75%;
    margin-top: 40px;
    display: flex;
    justify-content: center;
}
.rectangle {
  height: 55px;
  width: 75%;
  /* min-width: 700px; */
  max-width: 800px;
  background-color: #3E92CC;
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 5px rgb(119, 117, 117);
  text-align: center;
}
.about_me {
  display: flex;
  justify-content: center;
}
.about_me_title {
    position:absolute;
    display:flex;
}
.outer_rect {
    width: 75%;
    display: flex;
    justify-content: center;
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
}

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
    margin-top:15px;
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
    margin-top:15px;
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