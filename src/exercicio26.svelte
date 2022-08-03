<script>
	let scoops = 1;
	let flavours = [];
	let menu = ["Creme com chocolate", "Menta com chocolate", "Framboesa"];

	function join(flavours) {
		if (flavours.length === 1) {
            return flavours[0];
        }
        return `${flavours.slice(0, -1).join(', ')} e ${flavours[flavours.length - 1]}`;
	}
</script>

<h2>Quantidade</h2>

<label>
	<input type=radio bind:group={scoops} name="scoops" value={1}>
	Uma bola
</label>

<label>
	<input type=radio bind:group={scoops} name="scoops" value={2}>
	Duas bolas
</label>

<label>
	<input type=radio bind:group={scoops} name="scoops" value={3}>
	Três bolas
</label>

<h2>Sabores</h2>

{#each menu as flavour}
	<label>
		<input type=checkbox bind:group={flavours} name="flavours" value={flavour}>
		{flavour}
	</label>
{/each}

{#if flavours.length === 0}
	<p>Por favor, selecione pelo menos 1 sabor!</p>
{:else if flavours.length > scoops}
	<p>Erro! Você escolheu mais sabores do que quantidade de bolas</p>
{:else}
	<p>
		Você escolheu {scoops} {scoops === 1 ? "bola: " : "bolas: "} {join(flavours)}
	</p>
{/if}