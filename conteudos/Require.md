Traduzido para o português **`require`** pode ser lido como **`requerir`** e/ou **`pedir`**, o que ele basicamente faz é buscar informações que existem dentro de outros arquivos e isso pode ser MUITO útil pois ao invés de lidar com um código **ENOOOOORME** podemos dividir ele em pedaços, arquivo por arquivo e assim, deixamos mais fácil de ser entendido, então que tal aprender isso agora?

Antes de tudo é bom saber que, quando utilizamos o `require` para buscar informações de algum pacote que instalamos, apenas precisamos dizer o nome dele, pois por padrão o Node já compreende o que está dento da **`node_modules`**, mas isso não significa que devemos por algum arquivo lá ou alterar algum conteúdo, ok!?

Vamos fazer isso na prática, dentro do seu projeto crie um arquivo chamado **`aprendendo_require.js`** e um outro escrito **`conteudo_externo.js`**

Primeiro vamos começar pelo **`conteudo_externo.js`**

Imagine que temos um objeto chamado **`person`** e queremos deixar ele público para outros arquivos.
```js
const person = {
  name: 'Fagner',
  age: 19,
  hobbies: ['Trabalhar', 'Conversar', 'Ler', 'Escrever']
}
```
Bom, não é nada difícil, basta exportarmos utilizando o seguinte código:
```js
module.exports = person
```
Assim, estamos falando para o Node que, a informação **`person`** é pública e pode ser lida por outros arquivos

Agora que já estamos exportando nosso objeto, vamos agora acessar ele pelo arquivo **`aprendendo_require.js`**
```js
const conteudo_externo = require('./conteudo_externo.js')

console.log(`Olá, me chamo ${conteudo_externo.name}!`)
console.log(conteudo_externo)

// => Olá, me chamo Fagner!
// => {
// =>   name: 'Fagner',
// =>   age: 19,
// =>   hobbies: ['Trabalhar', 'Conversar', 'Ler', 'Escrever']
// => }
```
Mas espera um pouco, por que no exemplo foi utilizado este **`./`** no começo do require?
Bom, quando vamos buscar por um arquivo precisamos informar onde ele está, então segue abaixo alguns exemplos pra você entender direitinho! :)

Supondo que você vai utilizar o **`require`** e você está no arquivo **`index.js`**

```
📁 PastaPrincipal
 | - 📝 cores.js
 | - 📁 PastaSecundária
 | - - - 📝 pessoas.js
 | - - - 📁 PastaTerciária
 | - - - - - 📝 carros.js
 | - - - - - 📝 index.js
```

```js
/* Arquivos na mesma pasta "./" */
const carros = require('./carros.js')

/* A partir daqui, a cada pasta que quiser retornar é mais um "../" */
/* Arquivos na pasta anterior "../" */
const pessoas = require('../pessoas.js')

/* Duas pastas de distância */
const cores = require('../../cores.js')
```

