<script>
    import Profilepic from '../img/profilepic.jpg'
</script>
<br>
<section class="about_me">
    <!-- <div class= "aboutmebackground"> -->
        <div class="rectangle">
            <img class="profile_pic" src={Profilepic} alt="Brodie smiling">
            </div>
    <!-- </div> -->
    <h1 class="about_me_title">Hi, I'm Brodie Peif</h1>
</section>
    

<style>
.profile_pic {
    border-radius: 20%;
    width: 220px;
    height: 250px;
}
.about_me {
    width: 100%;
    height: 250px;
}
.rectangle {
  position:relative;
  top: 45%;
  left: 45%;
  height: 50px;
  width: 500px;
  background-color: #130fe6;
}
h1 {
    text-align: right;
    position:relative;
}
</style>