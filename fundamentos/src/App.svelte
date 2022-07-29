<script>
    import Router from "svelte-spa-router"
    import exercicio1 from "./exercicio1.svelte"
    import exercicio2 from "./exercicio2.svelte"
    import exercicio3 from "./exercicio3.svelte"
    import exercicio4 from "./exercicio4.svelte"
</script>

<Router routes={{
    "/exercicio1": exercicio1,
    "/exercicio2": exercicio2,
    "/exercicio3": exercicio3,
    "/exercicio4": exercicio4
}}></Router>