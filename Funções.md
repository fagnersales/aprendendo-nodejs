# O que é uma função em JavaScript?

Uma função nada mais é do que um **conjunto de códigos** que realiza alguma ação ao ser invocada, podendo ou não retornar algum valor ao finalizar. O propósito de utilizar funções é te possibilitar a fazer **MAIS** código em **MENOS** tempo e claro, lhe permitindo também fazer **códigos facilmente legíveis** e também de **fácil manutenção**!

Existem **MILHARES** de formas de se utilizar uma função, mas para você que está aprendendo, são poucas as coisas que você precisa aprender para voar longe com esse conhecimento, então, mãos a obra!

# Entendendo uma FUNÇÃO na PRÁTICA

Existem **duas** formas de se **definir** uma função, mas calma, abaixo terá esses exemplos, mas calma, não se preocupe com elas agora!

**Método Tradicional** 
```javascript
function name (param1, param2) {

}
```

**Método Arrow Function** 
```javascript
const name = (param1, param2) => {

}
```

Ok, já sabemos o por que de uma função ser **importante**, sabemos como **defini-la**, mas... talvez você ainda não esteja convencido ou então não entendeu de fato, então vamos por a mão na massa!

No exemplo abaixo vamos fazer com que apareça no terminal mensagens cumprimentando outras pessoas, primeiro fazendo de uma forma complicada e após utilizando **funções**!

```javascript
console.log('Olá Rafael, seja bem-vindo!')
console.log('Olá Lucas, seja bem-vindo!')
console.log('Olá Paloma, seja bem-vinda!')
console.log('Olá Diego, seja bem-vindo!')
console.log('Olá Eduarda, seja bem-vinda!')
console.log('Olá Maryane, seja bem-vinda!')

// => Olá Rafael, seja bem-vindo!
// => Olá Lucas, seja bem-vindo!
// => Olá Paloma, seja bem-vinda!
// => Olá Diego, seja bem-vindo!
// => Olá Eduarda, seja bem-vinda!
// => Olá Maryane, seja bem-vinda!

```

Ok... Isso foi meio chato de se fazer, vamos tentar fazer **utilizando funcões** agora!

```javascript

function cumprimentar (nome, sexo) {
    if (sexo == 'H') {
        console.log(`Olá ${nome}, seja bem-vindo!`)
    }

    if (sexo == 'M') {
        console.log(`Olá ${nome}, seja bem-vinda!`)
    }
}

cumprimentar('Rafael', 'H')
cumprimentar('Lucas', 'H')
cumprimentar('Paloma', 'M')
cumprimentar('Diego', 'H')
cumprimentar('Eduarda', 'M')
cumprimentar('Maryane', 'M')

// => Olá Rafael, seja bem-vindo!
// => Olá Lucas, seja bem-vindo!
// => Olá Paloma, seja bem-vinda!
// => Olá Diego, seja bem-vindo!
// => Olá Eduarda, seja bem-vinda!
// => Olá Maryane, seja bem-vinda!
``` 
Bom, você pode ver que o resultado é o **mesmo**, mas me diga, qual foi **mais fácil** de escrever e/ou mais **compreensível**?

Talvez você ainda não esteja convencido, então, vamos elevar o nível de nossos exemplos.
Nesse contexto, iremos criar uma função que recebe um texto simples e o transforma, colocando a primeira letra com caractere em maiúsculo, adiciona um ponto no final da frase e remove todos os espaços a mais!

~~Não se preocupe com o conteúdo do código, a ideia aqui é lhe mostrar como funções podem ser uma mão na roda!~~

```javascript

function embelezarTexto(texto) {
    const espacosRemovidos = texto.trim()
    const primeiraMaiuscula = espacosRemovidos[0].toUpperCase() + espacosRemovidos.substring(1)
    
    if (primeiraMaiuscula[primeiraMaiuscula.length - 1] == '.') {
        const textoCompleto = primeiraMaiuscula
        return textoCompleto
    } else {
        const textoCompleto = primeiraMaiuscula + "."
        return textoCompleto
    }
}


console.log(
    embelezarTexto('adoraria comer uma maçã'),
    embelezarTexto('um dia quero poder voar'),
    embelezarTexto('esse conteúdo é massa')
)

// => Adoraria comer uma maçã.
// => Um dia quero poder voar.
// => Esse conteúdo é massa.
```

Imagine a **infinidade** de coisas que você pode fazer utilizando **funções**!
