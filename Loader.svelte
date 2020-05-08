<script>
export let color="tomato";
export let width="5";
export let size=50;
</script>
<div class="wrapper">
<div class="loader" style='border-top: {width}px solid {color};border-width:{width}px;width:{size}px;
  height:{size}px;'></div>
</div>


<style>

.loader {
    text-align: center;
    margin:10px auto;
  border:solid #f3f3f3;
  border-radius: 50%;
  
  -webkit-animation: spin 2s linear infinite; /* Safari */
  animation: spin 2s linear infinite;
}

/* Safari */
@-webkit-keyframes spin {
  0% { -webkit-transform: rotate(0deg); }
  100% { -webkit-transform: rotate(360deg); }
}

@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}
</style>