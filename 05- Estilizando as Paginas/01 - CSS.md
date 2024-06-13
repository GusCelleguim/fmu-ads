# INICIANDO CSS

CSS (Cascading Style Sheets ou Folhas de Estilo em Cascata) é a linguagens de marcação (não de programação, assim como o HTML) responsável por adicionar estilos em nossas páginas feitas com HTML, como cores, tamanhos, posicionamentos e entre outros. Sem ele, as páginas são apenas um grupo de textos, links e imagens.

1. Criar um arquivo CSS. A primeira coisa que precisamos fazer é criar um arquivo CSS do qual nossa página HTML possa obter seu estilo. Então em seu editor de código basta você criar um novo arquivo chamado ele de `style.css`. Lembre-se que o nome pode ser qualquer um, mas precisar ter o .css no formato do arquivo.

2. Linkar seu CSS no HTML. Depois de criado precisamos conectar nosso arquivo style.css no documento HTML. Dentro da tag do documento HTML, vamos adicionar uma tag para conectar a nossa nova folha de estilo.

```md
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css"> //a  Link do Css no documento 
    <title>Document</title>
</head>
```

3. Chame e dê estilo aos elementos. Experimente selecionar um elemento e estilizá-lo.

Declaração do Css 

```Css

.Section s-hero (Seletor) {
Color(atributo): #00f(Valor);
Font-Size(atributo): 26px(valor da medida do elemento);
}

obs: sempre utilizar ;(ponto e virgula apos colocar os elementos)

```

Acabamos de chamar todas tags `<h1>` do nosso documento HTML e adicionar o tamanho da fonte para 26px e com a cor azul (sempre atualize a página em seu navegador assim que aplicar algo novo em seu arquivo CSS ou HTML).