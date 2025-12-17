---
layout: project
show_home: true

title: Aventura na Trilha Lagoa da Mata
title_logo: assets/images/trilha/trilhaLagoa.png
banner_image: assets/images/trilha/trilhaMapa.png
banner_style: style7 # 1 to 7

image: assets/images/trilha/trilhaFotogrametria.png
description: Fotogrametria Realizada na trilha Lagoa da Mata para acréscimo ao jogo virtual.

highlights:
  - title: Menu
    description: Tela onde acontece a Entrada do jogador, ele coloca seu nome e entra na sala designada (atualmente fixada em 1)
  - title: Jogo
    description: Tela principal do jogo em realidade virtual, onde o jogador percorre a trilha
em formato de tabuleiro virtual. O avanço ocorre a partir do lançamento do dado,
permitindo a movimentação do peão ao longo dos ladrilhos. Durante o percurso,
o jogador interage com cartas de desafio, perguntas educativas, objetos
explorativos e elementos informativos do ambiente. As respostas, ações e
pontuações são registradas e enviadas ao servidor em tempo real via WebSocket, permitindo a análise posterior dos dados do jogo.
  - title: EndGame
    description: Tela onde acontece a Saida ou Reentrada do jogador no game, ele seleciona o botão e entra na sala em que estava (atualmente fixada em 1) ou sai do jogo.

spotlight:
  class: custom-right # first element orientation: custom-right, custom-left
  title: Cenas 360 Interativas
  image: assets/images/trilha/trilhaLagoa.png
  content: |
    O ambiente virtual objeto deste trabalho foi desenvolvido para uma experiência em 6DoF (“Six degrees of freedom”), em que a interação do jogador com o ambiente e seus respectivos movimentos são fundamentais. Partindo deste princípio, para desenvolver o ambiente em realidade virtual RV foi utilizado o Framework Unity 3D e, para a conexão entre jogadores, o nodeJS..
    
    O Ambiente Virtual 'Trilha' está disponível no GitHub.
  urls:
    Código: https://github.com/multisens/Jogo-Trilha-Lagoa-da-Mata
    Documentação: https://github.com/multisens/Jogo-Trilha-Lagoa-da-Mata/blob/main/README.md
---

## Descrição Declarativa

A versão em RV do jogo de tabuleiro “Aventura na Trilha da Lagoa da Mata”, desenvolvido pela equipe do Laboratório de Limnologia da UFRJ (doravante chamado de TLM) foi desenvolvida com a intenção de aprimorar a imersão do jogador, integrando características presentes na trilha para fazê-lo ter uma experiência mais próxima da realidade.

<br>

## Arquitetura

```mermaid
    flowchart LR
        User[Usuário]
        web[Acesso Web]
        Frontend[VR Game]
        Backend[Backend Node]
        DB[(Mock DB)]
        Monitor[Monitoramento em Tempo real da analise dos dados do jogo]
        NoteDB["Mockado para facilitação da exportação dos dados.<br/>
        Já há suporte para bancos de dados relacionais."]
        Front[Frontend para Análise]

        NoteDB -.-> Backend
        User --> Frontend
        Backend --> Frontend
        Backend --> Front --> Monitor
        Backend --> DB
        web --> Front
        Frontend -->|WebSocket| Backend
        Frontend -.->|Continuidade definida pelo usuário| Frontend
```

A arquitetura do Trilha foi desenvolvida a fim de permitir multíplas conexões ao backend, e este trata os dados tanto para exibição do Frontend para análise dos dados quanto para prosseguir com o jogo.
Apesar de atualmente o backend estar mockado, já possui suporte integrado e facilitado para inserção de um bd.
Esta estrutura prevê duas arquiteturas diferentes em torno do backend centralizado (possuindo suporte para descentralização). Sendo a arquitetura VR -> Backend a arquitetura em camadas, onde o jogo ocorre na primeira camada e na segunda ocorre a conexão do sistema a parte e na terceira são onde estarão mantidos dos dados contidos inicialmente no backend e a conexão backend -> frontend compondo a arquitetura   cliente - servidor.

## Estrutura do projeto
O projeto está estruturado em pastas de acordo com o seu destino seu tipo de objeto. Árvores, Rochas, Scripts,  Packages, Cenas e etc.
Cada pasta têm subpastas com as informações de onde vieram os objetos (criador e etc), excetos em casos de Fotogrametria, onde somos os criadores e estão em uma pasta de mesmo nome.


## Publicações

CRUZ, Lucas Rangel da; SANTOS, Nicole Cristina Vieira dos; SOUZA, Luiz André de; OLIVEIRA, Andressa dos Santos; SILVA, Marcelo Arêas Rodrigues da; SANTOS, Joel André Ferreira dos. Trails of Performance: A Study of Real Time Optimization Techniques in Heterogeneous Natural Environments for VR. In: SIMPÓSIO BRASILEIRO DE JOGOS E ENTRETENIMENTO DIGITAL (SBGAMES), 24. , 2025, Salvador/BA. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2025 . p. 714-725. DOI: https://doi.org/10.5753/sbgames.2025.10340.

## Trabalhos Futuros

No viés de trabalhos futuros ficam:
* Incrementos do módulo de multiplayer.
* Remoção do módulo de jogo de tabuleiro.
* Mudanças no carregamento do jogo, a fim de carregar as cenas com uma tela de load.
* Mudanças no cenário de Menu e Endgame.
* Adição de mais objetos explorativos e um mapa de busca com os objetos a serem encontrados.
