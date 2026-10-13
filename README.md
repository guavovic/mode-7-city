<p align="center">
  <img src="assets/icone.svg" alt="" width="160">
</p>

<h1 align="center">Mode 7 City</h1>

<p align="center">City builder em 16 bits feito em Unity, inspirado no <a href="https://pt.wikipedia.org/wiki/SimCity_(jogo_eletr%C3%B4nico_de_1989)">SimCity</a> de Super Nintendo (1991): o menu de escolha dos 1.000 mapas, o nome da cidade e do prefeito e, a partir daí, a cidade. O caminho é primeiro refazer a mecânica do SimCity inteira e, depois, remodelar o jogo com ideias e arte próprias.</p>

<p align="center">
  <b><a href="https://github.com/users/guavovic/projects/5">Quadro do projeto</a></b>
  &nbsp;•&nbsp;
  <a href="https://github.com/guavovic/mode-7-city/issues">Issues</a>
</p>

> [!NOTE]
> O código do jogo é privado. Aqui ficam a vitrine e as tarefas.

<img src="assets/arte-tela-de-titulo.png" alt="Tela de título: o letreiro MODE 7 CITY sobre uma cidade em Mode 7 que vai até o rio, com o Dr. Wright fazendo joinha e PRESS START no painel do HUD" width="100%">

<img src="assets/simcity-menu-e-mapa.gif" alt="No menu, o contador troca entre os mapas 000 e 003; depois de digitar o nome da cidade, a partida abre com o mapa escolhido e a câmera percorre e afasta o terreno de terra, floresta e água" width="100%">

<sub>A escolha entre os 1.000 mapas, o nome da cidade e o começo da partida.</sub>

## Destaques

- **Os 1.000 mapas:** o menu escolhe entre os 1.000 mapas do original, e a partida abre com o mapa escolhido.
- **Simulação no ritmo do original:** o relógio roda as fases da simulação como o SimCity, com mês e ano a partir de janeiro de 1900.
- **Mapa em dados:** o terreno é uma grade em C# puro, desenhada num Tilemap, e os 12.000 objetos que o mapa criava viraram um.
- **Regras conferidas por testes:** testes de arquitetura falham se aparecer singleton, busca de objeto por nome, `Resources` ou o input antigo.
- **Arte própria:** toda a arte vai ser refeita num estilo 16 bits próprio, com tiles de 16×16.

## Artes

Artes de divulgação montadas com os sprites, o HUD e o letreiro do próprio jogo, sobre a cidade do mapa 007. A vista inclinada em Mode 7 é das artes: no jogo ela ainda vai chegar.

<img src="assets/arte-caixa-snes.png" alt="Capa no estilo das caixas de Super Nintendo dos anos 90, com a cidade em Mode 7 no centro e o Dr. Wright apontando" width="100%">

<img src="assets/arte-aparelho-do-menu.png" alt="O aparelho do menu de escolha dos mapas mostrando MODE 7 CITY no visor e a cidade em Mode 7 na tela, ao lado da placa com o menu do jogo" width="100%">

<img src="assets/arte-telas-do-jogo.png" alt="Montagem com a escolha do mapa, a vista em Mode 7 e a partida vista de cima com o HUD, sobre a skyline noturna da tela de título" width="100%">

## Como está sendo feito

O jogo começou em 2024 como um protótipo dos menus e do mapa. Em 2026 ele foi reorganizado numa arquitetura própria para jogos Unity, antes de a mecânica da cidade começar, com cada decisão registrada num ADR.

- **Migração sem parar o jogo:** o código antigo foi trocado área por área, com o jogo abrindo em todo commit. De 29 violações das regras de arquitetura para zero.
- **Regras conferidas por testes:** testes de arquitetura varrem o código e falham se aparecer singleton, busca de objeto por nome, `Resources` ou o input antigo.
- **Uma feature por pasta:** cada parte do jogo tem o próprio assembly e os próprios testes, e as partes se falam por eventos e interfaces.
- **Mapa em dados:** o terreno é uma grade em C# puro, testada sem cena, desenhada num Tilemap. Os 12.000 objetos que o mapa criava viraram um.
- **Simulação no ritmo do original:** o relógio roda as fases da simulação como o SimCity, com mês e ano a partir de janeiro de 1900.
- **Arte própria:** toda a arte vai ser refeita num estilo 16 bits próprio, com tiles de 16×16.

## Créditos

- **SimCity** é marca da Maxis e da Electronic Arts; a versão de Super Nintendo foi publicada pela Nintendo. Mode 7 City é um projeto independente, sem ligação com elas.
- Enquanto a arte própria não fica pronta, o jogo usa provisoriamente sprites do original (extraídos por Paper Jorge, via [The Spriters Resource](https://www.spriters-resource.com/)) e os [Micropolis SNES tiles](https://opengameart.org/content/micropolis-snes-tiles) (*Tile set by usr_share, based on the assets from Micropolis*, GPL 3.0).

---

<sub>Feito por [Gustavo Victor](https://github.com/guavovic)</sub>
