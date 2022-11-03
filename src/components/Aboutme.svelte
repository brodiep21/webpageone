<script>
    import Profilepic from '../img/profilepic.jpg'
</script>
<section class="about_me">
    
    <div class="whitespace"></div>
    <div class="rectangle">
        <img class="profile_pic" src={Profilepic} alt="Brodie smiling">
        <h1 class="about_me_title">Hi, I'm Brodie Peif</h1></div>
    
    <div class="outer_rect">
        
    <div class="pic">
        </div>
    </div>
    
    
</section>
    

<style>
.pic {
    display: flex;
    margin-left: 20%;
    position: absolute;
    width: 100%;
}
.profile_pic {
    border-radius: 20%;
    width: 225px;
    height: 250px;
    box-shadow: 0px 6px 15px  grey;
    position: absolute;
    margin-left: 10%;
}
.about_me {
    width: 100%;
    height: 300px;
    margin-top:15px;
    display: flex;
}
.whitespace {
    position: relative;
    margin-top: 20px;
}
.rectangle {
  height: 50px;
  width: 75%;
  max-width: 700px;
  background-color: #3ad98c;
  border-radius:1em;
  position:absolute;
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.834)
}
.int_rect {
    height: 50px;
    width:100%;
    text-align: end;
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
    width: 100%;
}

h1.about_me_title {
   justify-content:right;
   margin-top: 11px;
   text-align: justify;
   width:100% inherit;
   margin-left: 60% ;
   text-shadow: 0px 1px 1px rgba(44, 44, 44, 0.341);
   font-family: sans-serif;
   color: rgba(0, 0, 0, 0.652);
}

</style>