<!-- O elemento de divisão <div> é um container genérico para conteúdo de fluxo, que de certa forma não representa nada. Ele pode ser utilizado para
agrupar elementos para fins de estilos (usando class ou id), ou porque eles compartilham valores de atributos, como lang. Ele deve ser utilizado somente
quando não tiver outro elemento de semântica (tal como <article> ou <nav>). -->

<script>
    let m = {x:0, y:0};

    function movimentoMouse(event) {
        m.x = event.clientX;
        m.y = event.clientY;
    }
</script>
<div on:mousemove={movimentoMouse}>
    A posição do mouse é: {m.x} x {m.y}
</div>

<style>
    div {width: 100%; height: 100%;}
</style>