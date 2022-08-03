<script>
    import Exercicio20b from "./exercicio20b.svelte";

    function handleMessage(event) {
        alert(event.detail.text);
    }
</script>

<Exercicio20b on:message={handleMessage}/>