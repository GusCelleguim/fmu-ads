Entendendo a sintaxe como vimos anteriomente como chamar o estilo em css temos que entender como funciona o estilo 

## Sintaxe
A sintaxe do CSS é bem simples. Primeiro precisamos indicar um seletor (pela tag, id ou class) e dentro das chaves inserimos os comandos referente à formatação, que são as propriedade e valor.

```CSS
Seletor {
	Propriedade : valorDaPropiedade;
}
```

### Comentarios 
Para adicionar um comentário em nosso documento CSS, é preciso utilizar o comando `/**/` . Portanto, todo o código que estiver dentro dessa tag não será executado.

```CSS
H1 {
/* color: blue; */ //isso aqui e um comentario em css 
}
```

Seletores : 

Okay, mas se eu tiver mais de um elemento  <p> quiser mudar a cor do texto só de um
?

É aí que entram os identificadores ID e Class  

-As Classes são uma forma de identificar um grupo de elementos. Através delas, pode-se atribuir formatação a VÁRIOS elementos de uma vez.

-O ID é uma forma de identificar UM elemento, e devem ser única para cada elemento. Através dele, pode-se atribuir formatação a um elemento em especial.

Para fazermos referência a uma Classe usando um . (ponto) com o nome da Classe e para fazermos referência a um id usando um # (hashtag) no lugar do . (ponto). Podemos ter os dois no mesmo elemento também

No Nosso  Html ficara assim o forma da class e id 

```html
<body>
	<p class="souClass">
	sou um elemento Class
	</p>
	
	<p id="souID">
	sou um elemento ID
	</p>
</body>
```

```CSS
.souClass{
color: red ;
}

#souID{
color: red;
}
```

