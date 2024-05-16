Variáveis são lugares na memória onde colocamos valores para podermos trabalhar com eles posteriormente. As variáveis são um dos fatores para mantermos o código dinâmico, fácil de ser lido e compreendido Isso é, uma vez armazenado um valor em uma memória podemos utilizar seu valor ao longo do nosso código.

No JavaScript não há necessidade de declarar o tipo da variável, mas isso não significa que ela não tem tipo. Isso torna o JavaScript uma linguagem de tipagem dinâmica, o tipo é inferido pelo valor do dado e a checagem (type checking) é feita em tempo de execução (runtime). Então se você tiver uma variável chamado “nome” com o valor de “iuri” e ao longo do nosso código mudar seu valor para 10, para o JavaScript isso está certo. Isso tem seus lados bons e ruins.

TIpos de variaveis :

String  Uma string é uma sequência de caracteres usados para representar texto. São declaradas usando aspas simples ou aspas duplas.

Number  Number é um tipo de dado numérico. O JavaScript não diferencia números inteiros, em ponto flutuante, double

Boleano  Um booleano é um tipo de dado lógico que pode ter apenas um de dois valores possíveis: true (verdadeiro) ou false (falso).


usamos elemento `typeof`  no js para descobrir qual tipo de dado e que estamos usando 

```js

var nome = 'gustavo'

var idade = 36

console.log (typeof nome,typeof idade);

```

Podemos somar as Strings 
```Js
var nome = 'Jessica Wohrath';
var idade = 18 ;
console.log('meu nome' + 'e' + nome + 'e tenho' + idade + 'anos')
```


exer em javascript 
```js
// Declarar uma variável com o seu nome

var nome = 'Gustavo'

  

// Declarar uma variável com a sua idade

var idade = 19

  

// Declarar uma variável com a sua comida

var food = 'lasanha'

  

// favorita e não atribuir valor

var favorita

  

// Atribuir valor a sua comida favorita

var comidaFavoritaEboa = true

console.log(comidaFavoritaEboa)

// Declarar 5 variáveis diferentes sem valores

  

var timerival,nomeDoPai,timeDocoracao,endereco

  

console.log(timerival,nomeDoPai,timeDocoracao,endereco)

```
