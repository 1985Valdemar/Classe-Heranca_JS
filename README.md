<h1 align="center"> 🚀 TURMA 1 - Treinamento K&L 💻 🛠️ </h1>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-orange" alt="Status" />
  <img src="https://img.shields.io/badge/Versão-1.0.0-blue" alt="Versão" />
</p>

# 🛠️ Bora Juntar Ferramentas Para Desenvolvimento

## 🚀🕹️🎮 Bora Decolar No Conhecimento em Classes e Herança em JS!

<p align="center"> <a href="https://kellab.com.br/" target="_blank">K&L</a> </p>

<p align="center">
<a href="#sobre">Sobre</a>&nbsp;&nbsp;&nbsp|&nbsp;&nbsp;&nbsp;
<a href="#tecnologia">Tecnologia</a>&nbsp;&nbsp;&nbsp|&nbsp;&nbsp;&nbsp;
<a href="#autores">Autores</a>.
</p>

---

# 📖 Sobre

## Treinamento Para Aprimorar Conhecimento
Este treinamento tem como base aprender e aprimorar conhecimento em JavaScript.

![Captura de tela 2024-09-24 140815](https://github.com/user-attachments/assets/6a8839bb-3a12-4cae-b4a0-d6ac13b39384)

<p align="center">Figura-07: Imagem Testando Código.</p>

---

# 💻 Exemplo de Código

### Classe Pessoa

```javascript
// CRIAR CLASSE PESSOA
class Pessoa {
    constructor(nome, dt_nascimento) {
        this.nome = nome;
        this.dt_nascimento = dt_nascimento;
    }

    imprimir() {
        return `${this.nome} ${this.dt_nascimento}`;
    }
}

// PERMITIR USAR DE FORA
module.exports = { Pessoa };
```

### Classe com Herança => Classe Pessoa Fisica

```javascript
// Chamar importação
const { Pessoa } = require('./pessoa');

// EXTENDS = HERDA DA CLASSE PESSOA OS DADOS
class PessoaFisica extends Pessoa {
    cpf;

    // Override reescrevendo
    imprimir() {
        console.log(`${super.imprimir()} CPF: ${this.cpf}`);
    }
}

// VAI LIBERAR O ACESSO EXTERNO
module.exports = { PessoaFisica };

```

### Index

```javascript
// Utilizando as classes
const { PessoaFisica } = require('./pessoaFisica');
const { PessoaJuridica } = require('./pessoaJuridica');

// Criar variável física para armazenar
let pf = new PessoaFisica('Frank', '14/04/2017');
pf.cpf = '053.555.798.85';

// Criar variável jurídica
let pj = new PessoaJuridica('K&L', '20/20/2024', '20202202020');
pj.cnpj = '15.462.356/0001-39';

// Chamando método para imprimir
pf.imprimir();
pj.imprimir();

```

### 🛠️ Tecnologia
## Esse projeto foi desenvolvido com as seguintes tecnologias:

Visual Studio Code
Git e GitHub
HTML
CSS
JavaScript


✍️ Autores
Valdemar


