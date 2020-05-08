<script>
export let card_title='';
</script>
<div class="card">
<h4 class="title">
{card_title}
</h4>
    <slot></slot>
</div>

<style>
.title{
    color: rgb(173, 173, 173);
    margin:0;
    margin-bottom: 10px;
    padding:0;
}
.card{
    background-color: white;
    padding:20px;
    border-radius: 6px;
    box-shadow: 0px 2px 4px rgba(0,0,0,0.1);
    border:1px rgb(243, 243, 243) solid;
}
</style>