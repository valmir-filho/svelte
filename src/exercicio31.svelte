<script>
    let width;
    let height;
    let size = 42;
    let text = "Edite-me";
</script>

<input type= range bind:value={size}>
<input bind:value={text}>

<p>Tamanho: {width} pixels x {height} pixels</p>

<div bind:clientWidth={width} bind:clientHeight={height}>
    <span style="font-size: {size}px"> {text}</span>
</div>

<style>
    input {display: block;}
    div {display: inline-block;}
    span {word-break: break-all;}
</style>