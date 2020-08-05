Traduzido para o português `Slice` seria o mesmo que `pedaço`, então quando utilizamos esse método, estamos na verdade pegando um pedaço de algo.

A utilização desse método é bem simples, o primeiro parâmetro significa onde você quer **começar** a cortar sua fatia e o segundo (opcional) onde você quer **terminar** se o segundo não for informado, ele irá cortar até onde for possível!

> Observação: A posição é considerada **zero-based** então, ao fazer a contagem de onde quer cortar, você precisa começar com `0`
> Observação: Este metodo não vai alterar a `Array` utilizada! Ele irá lhe trazer uma nova!

### Exemplo com Array (Conjunto de Elementos):
```javascript
const animais = ["Dog", "Cat", "Bird"]
                   0      1      2
const novoAnimais = animais.slice(1)

console.log(novoAnimais)
// => ["Cat", "Bird"]
```

### Exemplo com String (Texto): 
```javascript
const frase = "Olá mundo!"
               0123456789

const novaFrase = frase.slice(3)

console.log(novaFrase)
// => mundo!
```

### 

Espero que tenha aprendido!
