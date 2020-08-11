Traduzindo para o português **`If`** equivale à **`Se`**, então no contexto de programação, queremos saber se uma **`condição`** é verdadeira e então fazer algo, vamos aos exemplos, mas antes, vamos ver a estrutura de um **`IF`**

### Estrutura:
```javascript
if (condição) {
  // código a ser executado se a condição for verdadeira
}
```

Agora que já sabemos a **`estrutura básica`** de um **`if`**, vamos fazer alguns exemplos, onde há condições **`VERDADEIRAS`** `(Truthy)` e condições **`FALSAS`** `(Falsy)` 

### Exemplo (If):
```javascript
// Condição VERDADEIRA (Truthy)

if (10 + 10 === 20) {
  console.log('10 + 10 === 20!')
}

// Condição FALSA (Falsy)

if (10 + 15 === 10) {
  console.log('10 + 15 === 10!')
}

// Resultado (Terminal):
// => 10 + 10 === 20!
```

> Apenas condições verdadeiras terão o escopo (conteúdo dentro das chaves { ... })código lido!

Isso não é tudo que podemos fazer utilizando **`If`**, existem outras variações que podemos utilizar, chamadas: **`else`** e **`else if`**

## `if...else`

O **`if...else`** vai basicamente, ler o escopo **`else`** apenas se o **`if`** for falso!

### Exemplo:
```javascript
// Falsy
if (10 + 10 === 30) {
  console.log('A condição 10 + 10 === 30 é verdadeira!')
} else {
  console.log('A condição 10 + 10 === 30 NÃO é verdadeira!')
}

// Resultado (Terminal):
// => A condição 10 + 10 === 30 NÃO é verdadeira!
```

### Exemplo²:
```javascript
// Truthy
if (10 + 10 === 20) {
  console.log('A condição 10 + 10 === 20 é verdadeira!')
} else {
  console.log('A condição 10 + 10 === 20 NÃO é verdadeira!')
}

// Resultado (Terminal):
// => A condição 10 + 10 === 20 é verdadeira!
```

## `if...else if`

A diferença deste para o **`if...else`**, é que ele só irá ler o código dele se a condição anterior for **`Falsy`** e a condição **dele** for verdadeira!

### Exemplo:
```javascript
// Truthy
if (15 + 15 === 30) {
  console.log('A condição 15 + 15 === 30 é verdadeira!')
} else if (10 + 10 === 20) {
  console.log('A condição 10 + 10 === 20 é verdadeira!')
}

// Resultado (Terminal):
// => A condição 15 + 15 === 30 é verdadeira!
```

Como você pode ver, apenas o primeiro if foi lido e o segundo não! Isto é por que, o **`else if`** só vai ser lido quando o if anterior for falso!

### Exemplo²:
```javascript
// Falsy
if (15 + 10 === 50) {
  console.log('A condição 15 + 10 === 50 é verdadeira!')
} else if (10 + 10 === 20) {
  console.log('A condição 10 + 10 === 20 é verdadeira!')
}

// Resultado (Terminal):
// => A condição 10 + 10 === 20 é verdadeira!
```

Se você entendeu como utilizar todos os **`ifs`**, saiba que você pode juntar todos eles também, vamos a alguns exemplos em que utilizamos todos eles!

```javascript
if (150 + 150 === 320) {
  console.log('If!')
} else {
  console.log('Else!')
}

// => Else!
```

```javascript
if (150 + 150 === 320) {
  console.log('If!')
} else if (100 + 100 === 200) {
  console.log('Else if!')
} else {
  console.log('Else!')
}

// => Else if!
```

> Obs: `else if` só funcionará depois de um `if` ou outro `else if`
> Obs2: `else` só funcionará depois de um `if` ou de um `else if`
