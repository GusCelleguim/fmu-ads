O Grid Layout é um sistema de layout CSS bidimensional que permite a criação de layouts complexos de uma maneira mais simples e intuitiva. Aqui estão algumas das principais propriedades e conceitos do Grid Layout, explicados com exemplos:

### 1. display: grid;

Define o elemento como um contêiner de grade.

```css
.container {
  display: grid;
}
```

### 2. display: inline-grid;

Define o elemento como um contêiner de grade, mas com comportamento inline.

```css
.container {
  display: inline-grid;
}
```

### 3. display: subgrid;

Para grids dentro de grids (ainda não suportado por todos os navegadores).

```css
.sub-container {
  display: subgrid; /* Uso futuro, atualmente você pode usar display: grid; */
}
```

### 4. grid-template-columns: 100px 100px 100px 100px;

Cria quatro colunas de 100px de largura cada.

```css
.container {
  display: grid;
  grid-template-columns: 100px 100px 100px 100px;
}
```

### 5. grid-template-columns: 1fr 2fr;

Cria duas colunas, sendo a segunda com o dobro do tamanho da primeira.

```css
.container {
  display: grid;
  grid-template-columns: 1fr 2fr;
}
```

### 6. grid-template-columns: minmax(200px, 1fr) 1fr 1fr;

Cria três colunas, sendo a primeira com no mínimo 200px de largura e no máximo 1fr.

```css
.container {
  display: grid;
  grid-template-columns: minmax(200px, 1fr) 1fr 1fr;
}
```

### 7. grid-template-columns: repeat(3, 1fr);

Cria três colunas com 1fr de tamanho cada.

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

### 8. grid-template-columns: repeat(auto-fit, minmax(100px, auto));

Cria automaticamente um número total de colunas que acomode itens com no mínimo 100px de largura.

```css
.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(100px, auto));
}
```

### 9. grid-template-rows: 50px 100px 50px 150px;

Cria quatro linhas no grid com tamanhos específicos.

```css
.container {
  display: grid;
  grid-template-rows: 50px 100px 50px 150px;
}
```

### 10. grid-template-rows: 1fr 2fr;

Cria duas linhas, sendo a segunda com cerca de duas vezes o tamanho da primeira.

```css
.container {
  display: grid;
  grid-template-rows: 1fr 2fr;
}
```

### 11. grid-template-areas:

Define áreas nomeadas no grid para facilitar o posicionamento de itens.

```css
.container {
  display: grid;
  grid-template-areas: 
    "logo nav nav"
    "sidenav content advert"
    "sidenav footer footer";
}

.logo {
  grid-area: logo;
}

.nav {
  grid-area: nav;
}

.sidenav {
  grid-area: sidenav;
}

.content {
  grid-area: content;
}

.advert {
  grid-area: advert;
}

.footer {
  grid-area: footer;
}
```

### 12. gap: 20px;

Define o espaço entre os elementos do grid (linhas e colunas).

```css
.container {
  display: grid;
  gap: 20px;
}
```

### 13. column-gap: 20px;

Define o espaço entre as colunas.

```css
.container {
  display: grid;
  column-gap: 20px;
}
```

### 14. row-gap: 20px;

Define o espaço entre as linhas.

```css
.container {
  display: grid;
  row-gap: 20px;
}
```

### Exemplo Completo

Aqui está um exemplo completo que demonstra várias dessas propriedades:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    .container {
      display: grid;
      grid-template-areas: 
        "logo nav nav"
        "sidenav content advert"
        "sidenav footer footer";
      grid-template-columns: 1fr 3fr 1fr;
      grid-template-rows: auto 1fr auto;
      gap: 10px;
    }
    .logo {
      grid-area: logo;
      background-color: lightblue;
      padding: 20px;
    }
    .nav {
      grid-area: nav;
      background-color: lightgreen;
      padding: 20px;
    }
    .sidenav {
      grid-area: sidenav;
      background-color: lightcoral;
      padding: 20px;
    }
    .content {
      grid-area: content;
      background-color: lightgoldenrodyellow;
      padding: 20px;
    }
    .advert {
      grid-area: advert;
      background-color: lightpink;
      padding: 20px;
    }
    .footer {
      grid-area: footer;
      background-color: lightgray;
      padding: 20px;
    }
  </style>
  <title>Grid Layout Exemplo</title>
</head>
<body>
  <div class="container">
    <div class="logo">Logo</div>
    <div class="nav">Nav</div>
    <div class="sidenav">Sidenav</div>
    <div class="content">Content</div>
    <div class="advert">Advert</div>
    <div class="footer">Footer</div>
  </div>
</body>
</html>
```

Este exemplo cria um layout de página com um cabeçalho, navegação, barra lateral, conteúdo principal, anúncio e rodapé, todos organizados em um grid.
