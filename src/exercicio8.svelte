<script>
    let count = 0;
    
    function incrementCount() {
        count += 1;
    }
</script>

<button on:click={incrementCount}>
    Clique {count} {count === 1 ? "vez" : "vezes"}
</button>