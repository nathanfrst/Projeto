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
