<script>
    function cliqueDoMouse() {
        alert("Clicado!");
    }
</script>

<button on:click|once={cliqueDoMouse}>
    Clique!
</button>