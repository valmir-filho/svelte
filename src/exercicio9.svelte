<script>
    let count = 0;
    let dobro = 0;

    function handleClick() {
        count += 1;
        dobro = count * 2;
    }
</script>

<button on:click={handleClick}>
    Clique {count} {count === 1 ? "vez" : "vezes"}
</button>

<p>O dobro de {count} é {dobro}</p>