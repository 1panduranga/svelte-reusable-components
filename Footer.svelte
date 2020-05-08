<script>
export let source="";
export let copyright='';
</script>
<footer>
{#if source!=""}
<div>
<img src={source} alt="footer_image" draggable="false" >
</div>
{/if}
{#if copyright!=''}
<div class="copyright">
<h6>
{copyright}
</h6>
</div>
{/if}
</footer>

<style>
footer{
    margin:220px auto 0px auto;
    padding:0px;
    opacity: 0.9;
    overflow: hidden;
    text-align: center;
}
.copyright{
    text-align: center;
    color:#aaa;
    font-size: 14px;
    padding:5px;
    display: inline-block;
    border-top:1px solid #ddd;

}
@media (max-width: 640px) {
		footer div img {
            height:100px;
            margin:100px 0px 0px 0px;
        }
	}

</style>