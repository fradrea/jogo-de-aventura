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
