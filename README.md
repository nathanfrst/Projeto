# 2D Side-Scroller

Um jogo 2D **side-scroller** desenvolvido em Java utilizando **Java Swing**.

O projeto está sendo desenvolvido como um projeto de estudo e prática de programação, com foco em Java, programação orientada a objetos, game loop, renderização 2D, entrada de teclado, animações e desenvolvimento de jogos.

## Sobre o jogo

Um jogo 2D de progressão lateral (*side-scroller*).

O jogador controla um personagem que deve avançar pelo cenário, interagir com o ambiente e enfrentar os desafios encontrados durante a progressão.

O conceito, a história e as mecânicas ainda estão em desenvolvimento.

## Tecnologias

* Java
* Java Swing
* AWT
* IntelliJ IDEA
* Git / GitHub

## Estrutura atual

O projeto utiliza uma arquitetura baseada em componentes:

```text
Main
 │
 └── JFrame
      │
      └── GamePanel
           ├── Game Loop
           ├── Player
           ├── Input
           ├── Camera
           └── Renderização
```

### Principais componentes

#### `Main`

Responsável pela inicialização da aplicação e configuração da janela do jogo.

#### `GamePanel`

Responsável pela área de renderização e pelo funcionamento principal do jogo.

Atualmente concentra:

* Game loop
* Atualização do estado do jogo
* Renderização
* Controle da câmera
* Entrada do jogador

#### `Player`

Responsável pelo personagem controlado pelo jogador.

Pretende-se implementar:

* Movimentação
* Direção
* Animações
* Sprites
* Física
* Interações

#### `KeyHandler`

Responsável pela leitura das entradas do teclado.

## Game Loop

O jogo utiliza um game loop baseado em uma thread própria.

O loop é responsável por atualizar o estado do jogo e solicitar sua renderização continuamente.

Fluxo simplificado:

```text
Game Loop
   │
   ├── update()
   │      └── Atualiza o estado do jogo
   │
   └── repaint()
          └── Renderiza o estado atual
```

A taxa de atualização atual está configurada para **120 FPS**.

## Sistema de câmera

O jogo possui uma câmera horizontal que acompanha o jogador.

A câmera será utilizada para permitir que o cenário se estenda além da área visível da tela, característica fundamental de um side-scroller.

Conceito:

```text
MUNDO DO JOGO
──────────────────────────────────────────────────────────────
        cenário              PLAYER
                              ↓
                  ┌─────────────────────┐
                  │    ÁREA VISÍVEL     │
                  └─────────────────────┘
                              ↓
                           CÂMERA
```

## Sistema de sprites

Os personagens utilizam imagens (`BufferedImage`) organizadas em arrays para representar diferentes frames de animação.

Exemplo conceitual:

```text
playerDown
[0] [1] [2] [3]

playerUp
[0] [1] [2] [3]

playerLeft
[0] [1] [2] [3]

playerRight
[0] [1] [2] [3]
```

O frame atual é selecionado durante a execução do game loop para produzir as animações do personagem.

## Resolução

O jogo utiliza uma resolução lógica baseada em tiles.

Configuração atual:

```text
Tile original: 32 × 32
Escala:        3×
Tile atual:    96 × 96

Tela:
16 × 12 tiles

Resolução lógica:
768 × 576
```

A resolução física da janela poderá ser diferente da resolução lógica, permitindo futuramente suporte a fullscreen e diferentes tamanhos de janela.

## Roadmap

O projeto ainda está em desenvolvimento.

### Fundação

* [x] Criar janela do jogo
* [x] Criar `GamePanel`
* [x] Implementar game loop
* [x] Implementar entrada de teclado
* [x] Criar personagem
* [x] Implementar câmera inicial
* [ ] Implementar sistema de escala
* [ ] Implementar fullscreen
* [ ] Implementar modo janela

### Player

* [ ] Movimentação horizontal
* [ ] Sistema de sprites
* [ ] Animações
* [ ] Gravidade
* [ ] Pulo
* [ ] Colisão
* [ ] Sistema de vida
* [ ] Interações

### Mundo

* [ ] Criar cenário
* [ ] Sistema de tiles
* [ ] Colisões do cenário
* [ ] Plataformas
* [ ] Background
* [ ] Parallax
* [ ] Sistema de fases

### Gameplay

* [ ] Inimigos
* [ ] Sistema de combate
* [ ] Objetivos
* [ ] Sistema de progressão
* [ ] Interface
* [ ] Menu principal
* [ ] Pause
* [ ] Game Over

### Finalização

* [ ] Efeitos sonoros
* [ ] Música
* [ ] Otimização
* [ ] Correção de bugs
* [ ] Testes
* [ ] Build final

## Objetivo do projeto

Além do desenvolvimento do jogo, este projeto tem como objetivo servir como estudo prático de desenvolvimento em Java.

Durante o desenvolvimento serão explorados conceitos como:

* Programação Orientada a Objetos
* Herança
* Encapsulamento
* Composição
* Estruturas de dados
* Threads
* Game loops
* Renderização 2D
* Eventos e entrada de usuário
* Gerenciamento de recursos
* Colisão
* Sistemas de coordenadas
* Câmera
* Animação
* Arquitetura de software

## Status

**Em desenvolvimento**

O projeto encontra-se em fase inicial de desenvolvimento. Mecânicas, história, arte e estrutura definitiva ainda podem sofrer alteraçõ
