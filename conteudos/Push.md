Traduzido para o português `Push` é o equivalente à `Empurrar`, mas imagine que seja algo como "`Empurrar para dentro`".
Push é uma função que existe apenas em `Array` (Conjunto de elementos) que você basicamente utiliza para empurrar para dentro deste conjunto novos elementos!

Obs: Isso irá alterar a **`Array`** principal!

### Exemplo:
```javascript
const perguntas = ["Qual seu nome?", "Tudo bem com você?"]

perguntas.push("Você tem um pet?")

console.log(perguntas)
// => ["Qual seu nome?", "Tudo bem com você?", "Você tem um pet?"]
```

Você pode adicionar qualquer tipo de elemento, seja um número, string, objeto, qualquer coisa!
