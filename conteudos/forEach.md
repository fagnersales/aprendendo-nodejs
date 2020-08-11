Traduzindo para o português **`forEach`** equivale à **`para cada`**, um método que existe apenas em `Array` e sua função é basicamente, executar uma outra `função anônima` passando como parametros: o `elemento atual`, `posição do elemento`, `array que foi utilizada`


### Exemplo
```javascript
const animals = ["Cachorro", "Gato", "Passáro"]

animals.forEach(function(elemento, posicao) {
  console.log(`O elemento ${elemento} está na posição ${posicao}`)
})
```
