<script>
import { bind } from "svelte/internal";

    let input;

    export function focus() {
        input.focus();
    }
</script>

<input bind:this={input}/>