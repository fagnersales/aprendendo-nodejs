Traduzido para o português `Join` significa `Juntar`, então quando utilizamos essa função estamos querendo juntar elementos de uma `Array` (conjunto de elementos), o legal dessa função é que você pode escolher algo para ficar entre as junções e no fim transformar num texto!

> Observação: A função `Join` não irá alterar a `Array`! Ela irá lhe trazer uma nova!

### Definição de array `palavras`:
```javascript
const palavras = ["Olá", "Mundo!"]
```

### Exemplo (1): 
```javascript
const novasPalavras = palavras.join()
console.log(novasPalavras)
// => Olá,Mundo!
```

### Exemplo (2):
```javascript
const novasPalavras = palavras.join('') // Separar por string vazia
console.log(novasPalavras)
// => OláMundo!
```

### Exemplo(3):
```javascript
palavras.join(' ') // Separar por um espaço em branco
const novasPalavras = 
console.log(novasPalavras)
// => Olá Mundo!
```

### Exemplo(4):
```javascript
const novasPalavras = palavras.join('-') Separar por um hífen
console.log(novasPalavras)
// => Olá-Mundo!
```

Com isso você tem infinitas possibilidades de trabalhar com uma array quando quiser transforma-lá num texto!
