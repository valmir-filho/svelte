<script>
    import Exercicio34b from "./exercicio34b.svelte";
    
    let field;
</script>

<inputField bind:this={field}/>

<button on:click={() => field.focus()}>Campo Foco</button>