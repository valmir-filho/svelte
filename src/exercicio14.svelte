<script>
    let x = 6;
</script>

{#if x > 10}
     <p>{x} é maior que 10</p>
{:else if x < 5}
    <p>{x} é menor que 5</p>
{:else}
    <p>{x} está entre 5 e 10</p>
{/if}