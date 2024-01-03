# Escrevendo-as-classes-de-um-Jogo
Escrevendo as classes de um Jogo
// Definição da classe Heroi
class Heroi {
  constructor(nome, idade, tipo) {
    this.nome = nome;
    this.idade = idade;
    this.tipo = tipo;
  }

  atacar() {
    let ataque = '';

    switch (this.tipo) {
      case 'mago':
        ataque = 'usou magia';
        break;
      case 'guerreiro':
        ataque = 'usou espada';
        break;
      case 'monge':
        ataque = 'usou artes marciais';
        break;
      case 'ninja':
        ataque = 'usou shuriken';
        break;
      default:
        ataque = 'não possui ataque definido';
    }

    console.log(`O ${this.tipo} atacou usando ${ataque}`);
  }
}

// Criando instâncias da classe Heroi
let heroi1 = new Heroi('Aragorn', 35, 'guerreiro');
let heroi2 = new Heroi('Gandalf', 150, 'mago');
let heroi3 = new Heroi('Bruce Lee', 32, 'monge');
let heroi4 = new Heroi('Hattori Hanzo', 40, 'ninja');

// Chamando o método atacar para cada herói
heroi1.atacar(); // Saída: O guerreiro atacou usando espada
heroi2.atacar(); // Saída: O mago atacou usando magia
heroi3.atacar(); // Saída: O monge atacou usando artes marciais
heroi4.atacar(); // Saída: O ninja atacou usando shuriken
