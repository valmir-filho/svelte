<script>
    let yes = false;
</script>

<label>
    <input type=checkbox bind:checked={yes}>
    Sim! Envie-me regularmente spam
</label>

{#if yes}
    <p>Obrigado! Vamos encher a sua caixa de entrada e vender seus dados pessoais...💀</p>
{:else}
    <p>Você deve optar por continuar. Se você não está pagando, você é o produto...💀</p>
{/if}

<button disabled={!yes}>
    Subscribe
</button>