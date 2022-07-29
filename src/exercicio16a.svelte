<!-- O método slice() retorna uma cópia de parte de um array a partir de um subarray criado entre as posições início e fim (fim não é necessário) de um
array original. O Array original não é modificado. -->

<script>
    import exercicio16b from "./exercicio16b.svelte";

    let comidas = [{id: 1, name: "maçã"}, {id: 2, name: "banana"}, {id: 3, name: "cenoura"}, {id: 4, name: "donut"}, {id: 5, name: "ovo"}];

    function handleClick() {
        
        comidas = comidas.slice(1);
    }
</script>

<button on:click={handleClick}}>
    Remova a 1ª comida
</button>

{#each comidas as comida}
    <exercicio16b name={comidas.name}/>
{/each}