<script>
    import DropMenu from './DropMenu.svelte'

    $: showMenu = false;
    
</script>

    <label for="check">
            <input type="checkbox" id="check" on:click={() => showMenu = !showMenu} /> 
            <span></span>
            <span></span>
            <span></span>
    </label>
    {#if showMenu}
    <DropMenu {showMenu}/>
    {/if}
<style>

label{
  display:flex;
  flex-direction:column;
  width:50px;
  cursor:pointer;
  position: absolute;
  margin-left: 5px;
  margin-top: .7em;
}

label span{
  background: var(--black);
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
  background-color: var(--red);
  transform:rotatez(45deg) translate(3px,-2px)
}


input[type="checkbox"]:checked ~ span:nth-of-type(2){
  
  transform-origin:top;
  width: 100%;
  background-color: var(--red);
  transform:rotatez(-45deg)
}


input[type="checkbox"]:checked ~ span:nth-of-type(3){
  
  transform-origin:bottom;
  width:50%;
  background-color: var(--red);
  transform: translate(21px,-4px) rotatez(45deg);

}

</style>