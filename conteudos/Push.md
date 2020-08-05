Traduzido para o português `Push` é o equivalente à `Empurrar`, mas imagine que seja algo como "`Empurrar para dentro`".
Push é uma função que existe apenas em `Array` (Conjunto de elementos) que você basicamente utiliza para empurrar para dentro deste conjunto novos elementos!

Obs: Isso não vai alterar a array! Ele irá lhe retornar uma nova array com os antigos elementos e os novos (juntos!)

### Exemplo (Errado!):
```javascript
const perguntas = ["Qual seu nome?", "Tudo bem com você?"]

perguntas.push("Você tem um pet?")

console.log(perguntas)
// => ["Qual seu nome?", "Tudo bem com você?"]
```

Como você pode ver no exemplo acima, empurramos para dentro de `perguntas` um novo texto e nada aconteceu, pois como eu disse, ele não altera a array, ele cria uma nova!

### Exemplo (Certo!):
```javascript
const perguntas = ["Qual seu nome?", "Tudo bem com você?"]

const novasPerguntas = perguntas.push("Você tem um pet?")

console.log(novasPerguntas)
// => ["Qual seu nome?", "Tudo bem com você?", "Você tem um pet?"]
```

Você pode adicionar qualquer tipo de elemento, seja um número, string, objeto, qualquer coisa!
