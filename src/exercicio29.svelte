<script>
	let todos = [{done: false, text: ""}, {done: false, text: ""}, {done: false, text: ""}];

	function add() {
		todos = todos.concat({done: false, text: ""});
	}

	function clear() {
		todos = todos.filter(t => !t.done);
	}

	$: remaining = todos.filter(t => !t.done).length;
</script>

<h1>TAREFAS</h1>

{#each todos as todo}
	<div class:done={todo.done}>
		<input
			type=checkbox
			bind:checked={todo.done}
		>

		<input
			placeholder="Digite a tarefa"
			bind:value={todo.text}
		>
	</div>
{/each}

<p>{remaining} tarefa(s) faltante(s)</p>

<button on:click={add}>
	Adicionar tarefa
</button>

<button on:click={clear}>
	Excluir tarefa(s) executada(s)
</button>

<style>
	.done {
		opacity: 0.4;
	}
</style>