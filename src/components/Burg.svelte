<script>
   
</script>

    <label for="check">
            <input type="checkbox" id="check"/> 
            <span></span>
            <span></span>
            <span></span>
          </label>

<style>

label{
  display:flex;
  flex-direction:column;
  width:50px;
  cursor:pointer;
}

label span{
  background: rgb(0, 84, 251);
  border-radius:10px;
  height: 4px;
  margin: 3px 0;
  transition: .7s  cubic-bezier(0.68, -0.6, 0.32, 1.6);
}

span:nth-of-type(1){
  width:40%;
  
}

span:nth-of-type(2){
  width:100%;
}


span:nth-of-type(3){
  width:20%;
 
}


input[type="checkbox"]{
  display:none;
}


input[type="checkbox"]:checked ~ span:nth-of-type(1){
  transform-origin:bottom;
  width:48%;
  transform:rotatez(45deg) translate(3px,-5px)
}


input[type="checkbox"]:checked ~ span:nth-of-type(2){
  
  transform-origin:top;
  width: 90%;
  transform:rotatez(-45deg)
}


input[type="checkbox"]:checked ~ span:nth-of-type(3){
  
  transform-origin:bottom;
  width:50%;
  transform: translate(23px,-5px) rotatez(45deg);

}
</style>