<script>
    import Exercicio33b from "./exercicio33b.svelte";

    let pin;
    $: view = pin ? pin.replace(/\d(?!$)/g, '•') : 'Digite o seu PIN';

    function handleSubmit() {
        alert(`PIN enviado: ${pin}`);
    }
</script>

<h2 style="color: {pin ? '#333' : '#ccc'}">{view}</h2>

<Exercicio33b bind:value={pin} on:submit={handleSubmit}/>