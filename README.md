//---------------------------------------------------------------
class DadosHeroi {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }
}
//---------------------------------------------------------------

let heroi = new DadosHeroi("jett", 17, "mago");

console.log(heroi);

//---------------------------------------------------------------

let atacar;

// Verifica o tipo do herói e define o ataque correspondente
switch (heroi.tipo) {
    case "mago":
        atacar = "magia";
        break;
    case "guerreiro":
        atacar = "espada";
        break;
    case "monge":
        atacar = "artes marciais";
        break;
    case "ninja":
        atacar = "shuriken";
        break;
    default:
        atacar = "ataque desconhecido";
}

console.log("O " + heroi.tipo + " atacou usando " + atacar);
