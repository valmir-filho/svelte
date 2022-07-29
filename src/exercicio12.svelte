<script>
    let usuario = {logar: false};

    function alternar() {
        usuario.logar = !usuario.logar;
    }
</script>

{#if usuario.logar}
<button on:click={alternar}>
    Logout
</button>
{/if}

{#if !usuario.logar}
<button on:click={alternar}>
    Login
</button>
{/if}