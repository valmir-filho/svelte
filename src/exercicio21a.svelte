<script>
    import Exercicio21c from "./exercicio21c.svelte";

    function handleMessage(event) {
        alert(event.detail.text);
    }
</script>

<Exercicio21c on:message={handleMessage}/>