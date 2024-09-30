# Jogo de Aventura - Classe Hero

Este repositório contém um projeto prático que implementa uma classe genérica chamada `Hero`, representando um herói em uma aventura. O objetivo deste projeto é demonstrar conceitos de programação orientada a objetos em JavaScript, incluindo a criação de classes, objetos, propriedades e métodos.

## Funcionalidades

- A classe `Hero` possui as seguintes propriedades:
  - `nome`: O nome do herói.
  - `idade`: A idade do herói.
  - `tipo`: O tipo do herói (ex: guerreiro, mago, monge, ninja).
  
- O método `atacar` exibe uma mensagem indicando o tipo de ataque do herói com base em seu tipo.

## Tipos de Ataque

Os tipos de ataque são definidos da seguinte forma:
- **Mago**: ataca usando magia.
- **Guerreiro**: ataca usando espada.
- **Monge**: ataca usando artes marciais.
- **Ninja**: ataca usando shuriken.

## Exemplo de Uso

```javascript
const hero = new Hero('Aragorn', 30, 'Guerreiro');
hero.atacar(); // Exibe: O guerreiro atacou usando espada.
// Classe Hero
class Hero {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    // Método para atacar
    atacar() {
        let ataque;

        // Determina o tipo de ataque com base no tipo do herói
        switch (this.tipo.toLowerCase()) {
            case 'mago':
                ataque = 'magia';
                break;
            case 'guerreiro':
                ataque = 'espada';
                break;
            case 'monge':
                ataque = 'artes marciais';
                break;
            case 'ninja':
                ataque = 'shuriken';
                break;
            default:
                ataque = 'ataque desconhecido';
        }

        // Exibe a mensagem de ataque
        console.log(`O ${this.tipo} atacou usando ${ataque}.`);
    }
}

// Exemplo de uso da classe Hero
const hero1 = new Hero('Aragorn', 30, 'Guerreiro');
const hero2 = new Hero('Gandalf', 200, 'Mago');
const hero3 = new Hero('Liang', 25, 'Monge');
const hero4 = new Hero('Kira', 22, 'Ninja');

// Chamando o método atacar para cada herói
hero1.atacar(); // O guerreiro atacou usando espada.
hero2.atacar(); // O mago atacou usando magia.
hero3.atacar(); // O monge atacou usando artes marciais.
hero4.atacar(); // O ninja atacou usando shuriken.
