<script>
    import Exercicio22b from "./exercicio22b.svelte";

    function handleClick() {
        alert("Botão clicado!");
    }
</script>

<Exercicio22b on:click={handleClick}/>
<Exercicio22b on:click={handleClick}/>