**Flexbox (Flexível Box Model)** é um módulo de layout CSS que permite a criação de layouts de página flexíveis e eficientes. Com ele, você pode alinhar e distribuir espaço entre os itens em um contêiner, mesmo quando o tamanho dos itens é desconhecido ou dinâmico. Abaixo, explicarei os principais conceitos e propriedades do Flexbox:

### 1. Display Flex

Para utilizar o Flexbox, você precisa definir um contêiner como um contêiner flexível usando a propriedade `display: flex;`.

```css
.container {
  display: flex;
}
```

### 2. Justify Content

A propriedade `justify-content` alinha os itens do contêiner ao longo do eixo principal (horizontalmente, por padrão).

- `flex-start`: Alinha os itens no início do contêiner.
- `flex-end`: Alinha os itens no final do contêiner.
- `center`: Centraliza os itens no contêiner.
- `space-between`: Distribui os itens com espaço igual entre eles.
- `space-around`: Distribui os itens com espaço igual ao redor deles.
- `space-evenly`: Distribui os itens com espaço igual entre eles, incluindo as extremidades.

```css
.container {
  display: flex;
  justify-content: center;
}
```

### 3. Align Items

A propriedade `align-items` alinha os itens ao longo do eixo transversal (verticalmente, por padrão).

- `stretch`: Estica os itens para preencher o contêiner (padrão).
- `flex-start`: Alinha os itens no início do contêiner.
- `flex-end`: Alinha os itens no final do contêiner.
- `center`: Centraliza os itens no contêiner.
- `baseline`: Alinha os itens na linha de base de seu conteúdo.

```css
.container {
  display: flex;
  align-items: center;
}
```

### 4. Flex Direction

A propriedade `flex-direction` define a direção do layout dos itens no contêiner.

- `row`: Alinha os itens em uma linha (horizontalmente, padrão).
- `row-reverse`: Alinha os itens em uma linha, mas na ordem inversa.
- `column`: Alinha os itens em uma coluna (verticalmente).
- `column-reverse`: Alinha os itens em uma coluna, mas na ordem inversa.

```css
.container {
  display: flex;
  flex-direction: column;
}
```

### 5. Flex Wrap

A propriedade `flex-wrap` controla se os itens devem ou não quebrar para uma nova linha.

- `nowrap`: Todos os itens são colocados em uma única linha (padrão).
- `wrap`: Os itens são quebrados em várias linhas, se necessário.
- `wrap-reverse`: Os itens são quebrados em várias linhas, mas na ordem inversa.

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

### 6. Inline-Block

A propriedade `display: inline-block;` é usada para elementos que devem ser exibidos em linha (como elementos `inline`), mas que podem ter propriedades de blocos aplicadas, como largura e altura.

```css
.item {
  display: inline-block;
  width: 100px;
  height: 100px;
}
```

### 7. Grid

O Grid Layout é um sistema de layout bidimensional que pode ser usado para criar layouts de grade complexos. Ele permite a criação de layouts tanto em linhas quanto em colunas.

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* Cria 3 colunas de tamanho igual */
  grid-gap: 10px; /* Espaçamento entre os itens */
}

.item {
  background-color: lightblue;
  padding: 20px;
}
```

### Exemplo Completo

Aqui está um exemplo completo que demonstra o uso do Flexbox:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100vh;
    }
    .item {
      background-color: lightblue;
      padding: 20px;
      margin: 10px;
    }
  </style>
  <title>Flexbox Exemplo</title>
</head>
<body>
  <div class="container">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
  </div>
</body>
</html>
```

Esse exemplo cria um contêiner flexível com três itens, espaçados igualmente entre si e alinhados ao centro verticalmente.

### Hotkeys

- **W:** Yes, Continue
  Confirm, advance to next step, proceed, again
- **A:** Alt
  2-3 alternative approaches, compare & rank
- **S:** Explain
  Explain each line of code step by step, adding descriptive comments
- **D:** Iterate, Improve, Evolve
  Note 3 critiques or edge cases, propose improvements 1,2,3