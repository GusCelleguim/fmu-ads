
|Operador|Descrição|Exemplo|
|---|---|---|
|==|Igual a (compara valor)|let isEqual = (x == y);|
|===|Igual a (compara valor e formato)||
|!==|Diferente de|let isNotEqual = (x != y);|
|>|Maior que|let isGreater = (x > y);|
|<|Menor que|let isLess = (x < y);|
|>=|Maior ou igual a|let isGreaterOrEqual = (x >= y);|
|<=|Menor ou igual a|let isLessOrEqual = (x <= y);|


```jsx
let marca = "Apple"
console.log(marca !== "Samsung")

// = é atribuição
// == é para comparar o valor
// === é para comparar o valor e o formato do conteúdo
// !== é diferente ?
```

```jsx
//guardar o valor em uma variável de resultado TRUE?FALSE
let marca = "Apple"
let resultado = marca === "Samsung"

console.log(resultado)
```

```jsx
//guardar o valor em uma variável de resultado TRUE?FALSE
let cpfBloqueado = "123.445.222-45"
let cpfUsuario = "222.111.222-09"
let ehCPFBloqueado = cpfUsuario === cpfBloqueado

console.log("O usuario está barrado ? " + ehCPFBloqueado)
```

```jsx
let CPFPermitido = "222.555.333-02"
let CPFDoUsuario = "222.555.333-02"

let ehBloqueado = CPFDoUsuario !== CPFPermitido

console.log("é um usuario invalido ? " + ehBloqueado)
```

```jsx
let idadeMinima = 18
let idadeUsuario = 18
let idadePermitidaValida = idadeUsuario >= idadeMinima

console.log(idadePermitidaValida)
```

```jsx
let idadeDeCorte = 50
let idadeUsuario = 50

let resultadoEhTerceiraIdade = idadeDeCorte <= idadeUsuario
console.log(resultadoEhTerceiraIdade)
```