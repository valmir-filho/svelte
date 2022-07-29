<script>
    let count = 0;
    
    $: if(count >= 10) {
        alert("O contador está perigosamente alto!");
        count = 9;
    }

    function handleClick() {
        count += 1;
    }
</script>

<button on:click={handleClick}>
    Clique {count} {count === 1 ? "vez" : "vezes"}
</button>