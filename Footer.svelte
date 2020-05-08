<script>
export let source;
</script>
<footer>
<div>
<img src={source} alt="footer_image" draggable="false" >
</div>
</footer>

<style>
footer{
    margin:180px 0px 0px 0px;
    padding:0px;
    opacity: 0.9;
    overflow: hidden;
}
@media (max-width: 640px) {
		footer div img {
            height:100px;
            
        }
	}
</style>