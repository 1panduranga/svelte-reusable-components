<header>
<div>
 <h4>
     <slot></slot>
 </h4>
</div>

</header>
   

<style>
div{
    text-align: center;
    background-color: rgb(255,230,194);
    border-radius: 6px;
    margin:0px auto;
}
header{
    text-align: center;
    
}
h4{
    padding:30px;
    margin:0px;
    color:brown;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-weight: normal;
}
@media (max-width: 640px) {
		h4{
            padding:10px;
        }
	}
</style>