<script>
	import {fade} from "svelte/transition";
	let visible = true;
</script>

<label>
	<input type="checkbox" bind:checked={visible}>
	Visível
</label>

{#if visible}
	<p transition:fade>
		Fades in and out
	</p>
{/if}