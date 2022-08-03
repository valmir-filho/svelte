<script>
    import {createEventDispatcher} from "svelte";

    const dispatch = createEventDispatcher();

    function sayHello() {
        dispatch("message", {text: "Olá!"});
    }
</script>

<button on:click={sayHello}>
    Clique para dizer "Olá"
</button>