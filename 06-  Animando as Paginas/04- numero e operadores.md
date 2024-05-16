# NÚMEROS
```js
var soma = 100 + 50; // 150
var subtracao = 100 - 50; // 50
var multiplicacao = 100 * 2; // 200
var divisao = 100 / 2; // 50
var expoente = 2 ** 4; // 16
var modulo = 14 % 5; // 4

```

## OPERADORES ARITMÉTICOS
```js
var soma = 100 + 50; // 150
var subtracao = 100 - 50; // 50
var multiplicacao = 100 * 2; // 200
var divisao = 100 / 2; // 50
var expoente = 2 ** 4; // 16
var modulo = 14 % 5; // 4
```

	-Lembrando que soma `+` em Strings serve para concatenar
	

## OPERADORES ARITMÉTICOS (STRINGS)

```js
var soma = '100' + 50; // 10050
var SomaTotalDaString = parseInt('100') + 50;
ou
var SomaTotalDaString = +'100' + 50;

var subtracao = '100' - 50; // 50
var multiplicacao = '100' * '2'; // 200

var divisao = 'Comprei 10' / 2; // NaN (Not a Number)
```

É possível verificar se uma variável é NaN ou não com a função `isNaN()`

## NAN = NOT A NUMBER

```js
var numero = 80;
var unidade = 'kg';
var peso = numero + unidade; // '80kg'
var pesoPorDois = peso / 2 // NaN (Not a Number)
```



## A ORDEM IMPORTA

Começa por multiplicação e divisão, depois por soma e subtração.

```js
var total1 = 20 + 5 * 2; // 30
var total2 = (20 + 5) * 2; // 50
var total3 = 20 / 2 * 5; // 50
var total4 = 10 + 10 * 2 + 20 / 2; // 40
```

COPIAR

> Parênteses para priorizar uma expressão

## OPERADORES ARITMÉTICOS UNÁRIOS

```js
var incremento = 5;
console.log(incremento++); // 5
console.log(incremento); // 6

var incremento2 = 5;
console.log(++incremento2); // 6
console.log(incremento2); // 6
```

COPIAR

> Mesma coisa para o decremento `--x`

## OPERADORES ARITMÉTICOS UNÁRIOS

O `+` e `-` tenta transformar o valor seguinte em número

```js
var frase = 'Isso é um teste';
+frase; // NaN
-frase; // NaN

var idade = '28';
+idade; // 28 (número)
-idade; // -28 (número)
console.log(+idade + 5); // 33 

var possuiFaculdade = true;
console.log(+possuiFaculdade); // 1
```



[https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_Operators](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_Operators) 
