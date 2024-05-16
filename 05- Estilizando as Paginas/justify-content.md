
Essa propriedade vai se encarregar de alinhar os itens dentro do
container de acordo com a direção pretendida e tratar da
distribuição de espaçamento entre eles.

OBS: caso seus itens esteja ocupando 100% de todo o container,
ela não se aplica

Possuem algumas variaçoes 

flex-start: início do container.
flex-end: final do container.
 center: ao centro do container.
 space-between: cria um espaçamento igual entre os
elementos.
space-around: os espaçamentos do meio são duas vezes
maiores que o inicial e final.

align itens 

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Fundamentos - Justify content</title>
    <style>
        .container {
            font-size: 16px;
            max-width: 400px;
            border: 1px solid black;
            margin: 0;
            display: flex;
            margin-bottom: 10px;
        }

        .item {
            background-color:blueviolet;
            margin: 5px;
            text-align: center;
            color: white;
        }

        .flex-start {
            justify-content: flex-start;
        }

        .flex-end {
            justify-content: flex-end;
        } 

        .center {
            justify-content: center;
        }

        .space-between {
            justify-content: space-between;
        }

        .space-around {
            justify-content: space-around;
        }

        .column {
            flex-direction: column;
            min-height: 200px;
        }


    </style>
</head>

<body>
    <h1>Row</h1>
    <p>Flex start</p>
    <section class="container flex-start">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>    
    </section>

    <p>Flex end</p> 
    <section class="container flex-end">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>   
    </section>

    <p>Center</p>
     <section class="container center">
         <div class="item">1</div>
         <div class="item">Item 2</div>
         <div class="item">Outro item 3</div>
         <div class="item">Item 4</div>
         <div class="item">Outro item 5</div>    
     </section>

    <p>Space between</p> 
    <section class="container space-between">
         <div class="item">1</div>
         <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Outro item 5</div>   
    </section>

    <p>Space around</p> 
    <section class="container space-around">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Outro item 5</div>   
    </section>

    <h1>Column</h1>
    <p>Flex start</p> 
    <section class="container flex-start column">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Outro item 5</div>   
    </section>

    <p>Flex end</p> 
    <section class="container flex-end column">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Outro item 5</div>   
    </section>
 
    <p>Center</p> 
    <section class="container center column">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Outro item 5</div>   
    </section>

    <p>Space between</p> 
    <section class="container space-between column">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Outro item 5</div>   
    </section>

    <p>Space around</p> 
    <section class="container space-around column">
        <div class="item">1</div>
        <div class="item">Item 2</div>
        <div class="item">Outro item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Outro item 5</div>   
    </section>

</body>
</html>
``` 

