<script>
import { createEventDispatcher} from 'svelte';
let dispatch=createEventDispatcher();
export let holder="";
const handleSubmit=(e)=>{
dispatch('gotSearch',e.target.elements[0].value.trim().toLowerCase())
e.target.reset();
}

</script>
<form on:submit|preventDefault={handleSubmit}>

<h6>
<slot></slot>
</h6>
<br>
<div>
<input type="text" name="search" placeholder={holder} class="browser-default" spellcheck="false" required='true' autocomplete="off">
</div>

</form>

<style>
form{
    margin:0px auto;
}
div{
text-align: center;
position: relative;
}
input[type="text"]{
    width:400px;
    margin:auto;
    border:1px solid rgb(197, 197, 197);
    border-radius: 10px;
    outline-width: 0px;
    padding:15px 20px;
    box-shadow: 0px 1px 3px rgba(0,0,0,0.1);
    
}
input[type="text"]:focus{
    border:1px solid #663535;
}
@media (max-width: 540px) {
	input[type="text"]{
    width:250px;
    height:20px;
}
	}

</style>