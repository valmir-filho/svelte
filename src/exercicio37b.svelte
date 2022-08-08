<script>
	import {count} from "./exercicio37e";

	function increment() {
		count.update(n => n + 1);
	}
</script>

<button on:click={increment}>
	+
</button>