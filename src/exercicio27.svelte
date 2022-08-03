<script>
    import {marked} from "marked";
    let value = "Algumas palavras estão em *itálico*, outras em **negrito**";
</script>

{@html marked(value)}

<textarea bind:value></textarea>

<style>
    textarea {width: 100%; height: 200px;}
</style>
