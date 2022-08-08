<script>
	import {count} from "./exercicio37e";
	import Incrementer from "./exercicio37b.svelte";
	import Decrementer from "./exercicio37c.svelte";
	import Resetter from "./exercicio37d.svelte";
</script>

<h1>Contador: {$count}</h1>

<Incrementer/>
<Decrementer/>
<Resetter/>