<!-- O elemento <p> representa um parágrafo. Eles são usados para agrupar conteúdos relacionados de qualquer tipo, como imagens e campos de um formulário. -->
<!-- O elemento <span> é um conteiner genérico em linha para conteúdo fraseado, que não representa nada por natureza. Ele pode ser usado para agrupar elementos para fins
de estilo (usando os atributos "class" ou "id"), ou para compartilhar valores de atributos como "lang". Ele deve ser usado somente quando nenhum outro elemento semântico
for apropriado. O <span> é muito parecido com o elemento <div>, entretando a <div> é um elemento de nível de bloco enquanto o <span> é um elemento em linha. -->

<script>
    const emojis = {maca: "🍎", banana: "🍌", cenoura: "🥕", donut: "🍩", ovo: "🥚"}

    export let name;

    const emoji = emojis[name];
</script>

<p>
    <span> O emoji para {name} é {emoji}.</span>
</p>

<style>
    p {
        margin: 0.8em 0;
    }
    span {
        display: inline-block;
        padding: 0.2em 1em 0.3em;
        text-align: center;
        border-radius: 0.2em;
        background-color: #FFDFD3;
    }
</style>
