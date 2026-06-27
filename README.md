# *Projeto Acadêmico Facultativo* #
## Jogo de Damas - Programação Orientada a Objetos
---
https://github.com/user-attachments/assets/675e5169-9fc2-4eec-8a0a-65ffa6db3048
---
### *MEMBROS DA EQUIPE*

    1. Allan Takeshi morimoto
    2. Geovana Gabriella Estrela Costa
    3. Heitor Alves dos Santos
    4. Kwan Wesley Goettems
    5. Thiago Muraro de Paula Gomes

## Explicação

Este projeto foi desenvolvido como trabalho discente efetivo da matéria **Programação Orientada a Objetos**.

A aplicação consiste em uma aplicação completa de um jogo de damas clássico utilizando a linguagem **Java**,
aplicando os principais conceitos da linguagem, como encapsulamento, herança, polimorfismo,
abstração, interfaces, tratamento de exceções e persistência de objetos.

O projeto foi dividido em dois programas principais:

* **P1 (CriadorPartida):** responsável por criar os objetos iniciais da aplicação a partir de um arquivo texto e persisti-los em formato binário.
* **P2 (ExecutarPartida):** responsável por restaurar os objetos persistidos e iniciar a interface gráfica do jogo.

---

# Contextualização

O jogo de damas é um jogo de estratégia para dois jogadores, disputado em um tabuleiro de 8x8 casas.

Cada jogador inicia a partida com 12 peças posicionadas nas casas escuras do tabuleiro.

O objetivo é capturar todas as peças adversárias ou impossibilitar o oponente de realizar movimentos válidos.

Durante o desenvolvimento foram implementadas as regras clássicas do jogo, incluindo:

* Movimentação diagonal das peças;
* Captura obrigatória;
* Capturas múltiplas (tomada em cadeia);
* Promoção para rainha;
* Movimentação especial da rainha;
* Vitória por eliminação das peças;
* Vitória por bloqueio de movimentos;
* Empate por ausência de capturas durante várias rodadas;
* Registro das jogadas em arquivo CSV.

---

# Sobre o Projeto

O sistema foi desenvolvido utilizando Java e a biblioteca Swing para construção da interface gráfica, de forma que ficasse visualmente amigavel para não programadores

A arquitetura foi organizada em diferentes pacotes, separando responsabilidades entre pacotes (modelo, persistência, interface gráfica e tratamento de exceções).

## Principais conceitos de Programação Orientada a Objetos utilizados

* Encapsulamento;
* Herança;
* Generalização e Especialização;
* Polimorfismo;
* Classe Abstrata;
* Interface;
* Tratamento de Exceções;
* Serialização de Objetos;
* Persistência em Arquivos;
* Organização em Pacotes.

## Estrutura do Projeto

```text
Trabalho_POO/JogodeDamas_2.50/JogodeDamas_2.5/JogodeDamas_2
src/
│
├── aplicacao/
│   ├── CriadorPartida.java
│   └── ExecutarPartida.java
│
├── gui/
│   ├── TelaJogo.java
│   └── TelaResultado.java
│
├── model/
│   ├── Partida.java
│   ├── Tabuleiro.java
│   ├── Peca.java
│   ├── PecaComum.java
│   ├── Rainha.java
│   ├── Movimento.java
│   ├── Jogador.java
│   └── ResultadoMovimento.java
│
├── persistencia/
│   ├── Serializador.java
│   ├── CsvManager.java
│   ├── LoggerPartida.java
│   └── LeitorJogadores.java
│
└── exceptions/
    ├── MovimentoInvalidoException.java
    └── CapturaObrigatoriaException.java
```

---

# Funcionalidades

* Interface gráfica em Java Swing;
* Tabuleiro 8x8;
* Movimentação válida das peças;
* Captura obrigatória;
* Capturas múltiplas;
* Promoção automática para rainha;
* Movimentação especial da rainha;
* Controle de turnos;
* Identificação de vitória;
* Identificação de empate;
* Registro das jogadas em arquivo CSV;
* Persistência da partida utilizando serialização;
* Tratamento de exceções personalizadas.

---

# Como Executar

## Requisitos

* Java JDK 17 ou superior;
* IDE Java (NetBeans, IntelliJ IDEA ou Eclipse, é possivel executar o programa no VS code, entretanto é necessário instalar algumas extensões para o funcionamento).

## Localização do diretório

* Primeiro: Abrir o arquivo Trabalho_POO;
* Segundo: Abrir a pasta JogosdeDamas_2.50;
* Terceiro: Abrir a pasta JogodeDamas_2;
* Quarto: Abrir a pasta src (diretório dos arquivos);

## Passo 1

Execute o programa:

```text
CriadorPartida.java
```

Este programa realiza as seguintes operações:

* Cria os objetos iniciais da partida;
* Inicializa o tabuleiro;
* Salva os dados em `dados.bin`.

---

## Passo 2

Execute o programa:

```text
ExecutarPartida.java
```

Este programa:

* Carrega o arquivo `dados.bin`;
* Restaura toda a partida em memória;
* Inicializa a interface gráfica;
* Permite a execução completa do jogo.

---

# Arquivos Gerados

Durante a execução são gerados os seguintes arquivos:

| Arquivo        | Descrição                              |
| -------------- | -------------------------------------- |
| dados.bin      | Objetos persistidos da partida         |
| resultado.csv  | Registro das jogadas e resultado final |

* Obs: os arquivos de saida .csv e .bin estão localizados na pasta JogodeDamas_2.50.

---

# Considerações Finais

O desenvolvimento deste projeto foi um desafio que possibilitou a aplicação na prática dos principais conceitos que estudamos em sala de aula.

Além da implementação das regras do jogo de damas, foram utilizados mecanismos de persistência, tratamento de exceções, organização em pacotes, serialização de objetos e construção de interfaces gráficas utilizando Java Swing.

Esse foi um desafio que nos possibilitou colocar em prática todo o conhecimento que obtivemos ao longo do curso, não foi fácil, em muitos momentos quebramos a cabeça
pra chegar no resultado atual, mas ficamos satisfeitos com oq conseguimos fazer.

O projeto atende aos requisitos propostos pelo professor.
