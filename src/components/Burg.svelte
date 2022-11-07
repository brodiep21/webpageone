<script>
  let menu = false;
  export function openMenu () {
    menu = !menu;
   }
</script>

    <label for="check">
            <input type="checkbox" id="check" on:click={openMenu}/> 
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
  background: #000000;
  border-radius:10px;
  height: 5px;
  margin: 3px 0;
  transition: .7s  cubic-bezier(0.68, -0.6, 0.32, 1.6);
}

span:nth-of-type(1){
  width:100%;
  
}

span:nth-of-type(2){
  width:100%;
}


span:nth-of-type(3){
  width:100%;
 
}


input[type="checkbox"]{
  display:none;
}


input[type="checkbox"]:checked ~ span:nth-of-type(1){
  transform-origin:bottom;
  width: 50%;
  background-color: rgb(255, 20, 20);
  transform:rotatez(45deg) translate(3px,-2px)
}


input[type="checkbox"]:checked ~ span:nth-of-type(2){
  
  transform-origin:top;
  width: 100%;
  background-color: rgb(255, 20, 20);
  transform:rotatez(-45deg)
}


input[type="checkbox"]:checked ~ span:nth-of-type(3){
  
  transform-origin:bottom;
  width:50%;
  background-color: rgb(255, 20, 20);
  transform: translate(21px,-4px) rotatez(45deg);

}
</style>