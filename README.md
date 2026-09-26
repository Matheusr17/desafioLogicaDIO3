# ⚔️ Escrevendo as Classes de um Jogo

Projeto desenvolvido como desafio prático da [Digital Innovation One (DIO)](https://www.dio.me/), com o objetivo de praticar conceitos fundamentais de JavaScript, principalmente **classes, objetos, métodos, variáveis, operadores e estruturas condicionais**.

## 🎯 Objetivo

Criar uma classe genérica que represente um herói de uma aventura, contendo:

- Nome
- Idade
- Tipo

O herói também possui um método `atacar()`, responsável por exibir uma mensagem de ataque de acordo com seu tipo.

## 🧙 Tipos de Herói

| Tipo | Ataque |
|---|---|
| Mago | Magia |
| Guerreiro | Espada |
| Monge | Artes marciais |
| Ninja | Shuriken |

## 💻 Tecnologias utilizadas

- JavaScript
- Programação Orientada a Objetos (POO)

## 🚀 Como executar

O código pode ser executado diretamente em um compilador online de JavaScript, como o **Programiz**.

Também é possível executar utilizando o Node.js no computador.

### Exemplo

```javascript
class Heroi {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    atacar() {
        let ataque;

        if (this.tipo === "mago") {
            ataque = "magia";
        } else if (this.tipo === "guerreiro") {
            ataque = "espada";
        } else if (this.tipo === "monge") {
            ataque = "artes marciais";
        } else if (this.tipo === "ninja") {
            ataque = "shuriken";
        }

        console.log(`o ${this.tipo} atacou usando ${ataque}`);
    }
}

let mago = new Heroi("Gandalf", 100, "mago");
let guerreiro = new Heroi("Aragorn", 35, "guerreiro");

mago.atacar();
guerreiro.atacar();