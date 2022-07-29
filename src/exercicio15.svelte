<!-- O elemento <ul> representa uma lista de itens sem ordem rígida, isto é, uma coleção de itens que não trazem uma ordenação numérica e as suas
posições, nessa lista, são irrelevantes. -->
<!-- O elemento <li> é usado para representar um item que faz parte de uma lista. Este item deve estar contido em um elemento pai: uma lista ordenada
<ol>, uma lista desordenada <ul>, ou um menu <menu> e representa uma única entidade dessa lista. Em menus e listas desordenadas a relação de
itens é exibida, normalmente, usando pontos de marcação (as bolinhas). Em listas ordenadas eles são, comumente, mostrados com algum contador
ascendente, como um número, ou letra à sua esquerda. -->
<!-- O elemento <a> com o atributo href cria-se um hiperligação nas páginas web, arquivos, endereços de emails, ligações na mesma página ou endereços
na URL. O conteúdo dentro de cada <a> precisará indicar o destino do link. -->

<script>
    let gatos = [{id: "J---aiyznGQ", name: "Keyboard Cat"}, {id: "z_AbfPXTKms", name: "Maru"}, {id: "OUtn3pvWmpg", name: "Henry Existencial"}];
</script>

<h1>Gatos famosos do Youtube</h1>

<ul>
    {#each gatos as {id, name}, i}
        <ul>
            <a target="_blank" href="https://www.youtube.com/watch?v={id}">
                {i + 1}: {name}
            </a>
        </ul>
    {/each}
</ul>