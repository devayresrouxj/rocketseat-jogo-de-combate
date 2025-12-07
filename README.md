![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

# ⚔️ Jogo de Combate RPG

Jogo de combate por turnos desenvolvido em Python utilizando os conceitos de Programação Orientada a Objetos.

## 📋 Sobre o Projeto

Este projeto foi desenvolvido durante as aulas do módulo **Programação Orientada a Objetos** da [Formação Python](https://www.rocketseat.com.br/formacao/python) da [Rocketseat](https://www.rocketseat.com.br/).

O objetivo é aplicar na prática os pilares da POO através da criação de um sistema de combate baseado em turnos, onde o jogador controla um herói que enfrenta inimigos em batalhas estratégicas.

## 🛠️ Tecnologias

- Python 3.x
- Módulo `random` (geração de dano aleatório)

## 🎮 Como Funciona

O jogo simula uma batalha por turnos entre um **Herói** (controlado pelo jogador) e um **Inimigo** (controlado pelo algoritmo). A cada turno, o jogador pode escolher entre um ataque normal ou um ataque especial, enquanto o inimigo responde automaticamente.

A batalha continua até que um dos personagens tenha sua vida reduzida a zero.

## ✨ Funcionalidades

- **Sistema de Combate por Turnos**: Batalhas estratégicas entre herói e inimigo
- **Ataque Normal**: Causa dano baseado no nível do personagem
- **Ataque Especial**: Habilidade única do herói com dano aumentado
- **Sistema de Dano Aleatório**: Combates mais dinâmicos e imprevisíveis
- **Sistema de Vida**: Gerenciamento de pontos de vida dos personagens
- **Sistema de Níveis**: Influencia no poder dos ataques
- **Detalhes dos Personagens**: Visualização de status durante a batalha
- **Condições de Vitória/Derrota**: Feedback ao final da batalha

## 🎯 Conceitos de POO Aplicados

### 🔒 Encapsulamento

- Atributos privados (`__nome`, `__vida`, `__nivel`)
- Métodos getters para acesso controlado aos atributos
- Proteção dos dados internos das classes

### 🧬 Herança

- Classe base `Personagem` com características comuns
- Classe `Heroi` herda de `Personagem` e adiciona habilidade especial
- Classe `Inimigo` herda de `Personagem` e adiciona tipo
- Reutilização de código através de herança

### 🔄 Polimorfismo

- Sobrescrita do método `exibir_detalhes()` nas classes filhas
- Método `super()` para estender funcionalidades da classe pai
- Comportamentos especializados mantendo interface comum

### 🎭 Abstração

- Classe `Jogo` como orquestradora da lógica de batalha
- Separação de responsabilidades entre classes
- Interface simples para interação complexa

### Boas Práticas POO

- Classes coesas com responsabilidades bem definidas
- Métodos com propósitos específicos
- Documentação com docstrings
- Nomenclatura clara e descritiva

## 🏗️ Estrutura do Projeto

```
📦 Jogo de Combate
├── 🎭 Personagem (Classe Base)
│   ├── Atributos: nome, vida, nivel
│   ├── Métodos: atacar(), receber_ataque(), exibir_detalhes()
│   └── Getters: get_nome(), get_vida(), get_nivel()
│
├── 🦸 Heroi (Herda de Personagem)
│   ├── Atributo adicional: habilidade
│   ├── Método especial: ataque_especial()
│   └── Sobrescrita: exibir_detalhes()
│
├── 👾 Inimigo (Herda de Personagem)
│   ├── Atributo adicional: tipo
│   └── Sobrescrita: exibir_detalhes()
│
└── 🎮 Jogo (Classe Orquestradora)
    ├── Gerencia herói e inimigo
    └── Controla fluxo da batalha
```

## 🚀 Como Executar

1. Certifique-se de ter o Python 3.x instalado:

```bash
python --version
```

2. Clone este repositório:

```bash
git clone https://github.com/devayresrouxj/rocketseat-jogo-de-combate.git
```

3. Navegue até o diretório do projeto:

```bash
cd rocketseat-jogo-de-combate
```

4. Execute o jogo:

```bash
python jogo.py
```

## 💡 Como Jogar

1. O jogo inicia automaticamente a batalha
2. A cada turno, você verá os detalhes dos personagens:
   ```
   Nome: Herói
   Vida: 100
   Nível: 5
   Habilidade: Super Força
   ```
3. Pressione ENTER para continuar
4. Escolha seu tipo de ataque:
   - **1**: Ataque Normal (dano: 2x a 4x o nível)
   - **2**: Ataque Especial (dano: 5x a 8x o nível)
5. O inimigo ataca automaticamente
6. A batalha continua até alguém ser derrotado

## 🎓 Aprendizados

Este projeto consolidou conhecimentos em:

- **Hierarquia de classes**: Criação de classes base e derivadas
- **Encapsulamento**: Proteção de atributos e uso de getters
- **Herança**: Reutilização de código e extensão de funcionalidades
- **Polimorfismo**: Sobrescrita de métodos para comportamentos especializados
- **Composição**: Classe `Jogo` gerencia objetos `Heroi` e `Inimigo`
- **Design de classes**: Separação de responsabilidades
- **Lógica de jogo**: Implementação de mecânicas de combate

## 📊 Exemplo de Combate

```
Iniciando batalha!

Detalhes dos Personagens:
Nome: Herói
Vida: 100
Nível: 5
Habilidade: Super Força

Nome: Morcego
Vida: 80
Nível: 5
Tipo: Voador

Pressione Enter para atacar...
Escolha (1 - Ataque Normal, 2 - Ataque Especial): 2
Herói usou a habilidade especial Super Força em Morcego e causou 35 de dano!
Morcego atacou Herói e causou 12 de dano!
```

## 📝 Licença

Este projeto está sob a licença MIT.

---

Desenvolvido com 💜 durante a Formação Python da Rocketseat
