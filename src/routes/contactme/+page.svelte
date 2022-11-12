<script>
	import { text } from "svelte/internal";
	import Nav from "/src/components/Nav.svelte"
	// import Burg from "/src/components/Burg.svelte"

</script>
<Nav/>
<!-- <Burg/> -->
<div class="formwrap">
	<div class="form">
		<li><h2>Your Name</h2>
			<input type='text' class='Name'></li>
		<li><h2>Subject</h2>
			<input type='text' class='Name'></li>
		
		<li><input type='text' class="body"></li>
	</div>
</div>



<style>
.formwrap {
	text-align: left;
    border-radius: 10px;
    background: radial-gradient(circle,  var(--purple) 5%, var(--veridian) 99%);
    box-shadow: 0px 1px 4px var(--grey);
    display: flex;
}
.form {
	padding-top: 80px;
	position:relative;
	
}
.form li {
	list-style: none;
}
.Name {
    width: 100;
	height: 30;
}
.body {
	margin-top: 20px;;
	min-width: 300px;
	height: 200px;
}
</style>