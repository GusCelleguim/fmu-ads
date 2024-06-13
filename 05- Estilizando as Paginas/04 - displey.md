O CSS `display` é uma das propriedades mais importantes para controlar o layout e o comportamento dos elementos HTML. A propriedade `display` define como um elemento será exibido na página e como ele se comportará em relação aos elementos ao seu redor. Aqui estão algumas das opções mais comuns:

**1. Display: block;**
Os elementos com `display: block` são exibidos como blocos. Eles ocupam toda a largura disponível do elemento pai e sempre começam em uma nova linha. Exemplos de elementos de bloco incluem `<div>`, `<h1>` a `<h6>`, `<p>`, e `<form>`.

Exemplo:
```css
.elemento-bloco {
  display: block;
}
```

**2. Display: inline;**
Os elementos com `display: inline` são exibidos na mesma linha que os elementos adjacentes, sem iniciar uma nova linha. Eles ocupam apenas a largura necessária para o seu conteúdo e não respeitam propriedades de largura e altura. Exemplos de elementos inline incluem `<span>`, `<a>`, `<strong>`, e `<em>`.

Exemplo:
```css
.elemento-inline {
  display: inline;
}
```

**3. Display: inline-block;**
Os elementos com `display: inline-block` combinam as características dos elementos de bloco e inline. Eles são exibidos na mesma linha que os elementos adjacentes (como inline), mas podem ter largura e altura definidas (como block). Isso é útil para criar layouts mais complexos.

Exemplo:
```css
.elemento-inline-bloco {
  display: inline-block;
}
```

**4. Display: flex;**
Os elementos com `display: flex` se tornam contêineres flexíveis, permitindo um layout mais eficiente e controlado dos seus elementos filhos. O Flexbox facilita a distribuição do espaço e o alinhamento dos itens dentro do contêiner, seja na direção horizontal ou vertical. É extremamente útil para layouts responsivos.

Exemplo:
```css
.container-flex {
  display: flex;
}
```

**5. Display: none;**
Os elementos com `display: none` são completamente removidos do fluxo do documento e não ocupam espaço na página. Eles não são visíveis e não afetam o layout dos outros elementos. Esta propriedade é útil para esconder elementos que você não deseja exibir, mas que ainda precisa manter no DOM por algum motivo.

Exemplo:
```css
.elemento-none {
  display: none;
}
```

Aqui está um exemplo completo ilustrando o uso dessas diferentes propriedades `display`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .bloco {
      display: block;
      width: 100%;
      background-color: lightblue;
    }

    .inline {
      display: inline;
      background-color: lightgreen;
    }

    .inline-bloco {
      display: inline-block;
      width: 100px;
      height: 50px;
      background-color: lightcoral;
    }

    .flex-container {
      display: flex;
      justify-content: space-around;
      background-color: lightgray;
    }

    .none {
      display: none;
    }
  </style>
  <title>Exemplo de Display</title>
</head>
<body>
  <div class="bloco">Este é um elemento de bloco.</div>
  <span class="inline">Este é um elemento inline.</span>
  <div class="inline-bloco">Este é um elemento inline-block.</div>
  <div class="flex-container">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
  </div>
  <div class="none">Este elemento está oculto.</div>
</body>
</html>
```

Neste exemplo, você pode ver como cada propriedade `display` afeta o layout dos elementos na página. O conhecimento dessas propriedades permite criar layouts mais flexíveis e sofisticados.