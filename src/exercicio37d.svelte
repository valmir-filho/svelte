<script>
	import {count} from "./exercicio37e";

	function reset() {
		count.set(0);
	}
</script>

<button on:click={reset}>
	zerar contador
</button>