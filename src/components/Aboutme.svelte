<script>
    import Profilepic from '../img/profilepic.jpg'
</script>
<br>
<section class="about_me">
    <div class="blank"></div>
    <div class="outer_rect">
        <h1 class="about_me_title">Hi, I'm Brodie Peif</h1>
        <img class="profile_pic" src={Profilepic} alt="Brodie smiling">
        <div class="rectangle">
        </div>
    </div>
    
    
</section>
    

<style>
.profile_pic {
    border-radius: 20%;
    width: 220px;
    height: 250px;
    display: flex;
    position:absolute;
}
.about_me {
    width: 100%;
    height: 250px;
}
.rectangle {
  object-position: 4em;
  height: 50px;
  width: 600px;
  background-color: #51a2ff;
  border-radius:1em;
  display:flex;
}
.about_me {
  display: flex;
  
}
.about_me_title {
    position:absolute;
    display:flex;
    width: 30%;
   padding
}
.outer_rect {
    justify-content:center;
}
.blank {
    width: 30%;
}

</style>