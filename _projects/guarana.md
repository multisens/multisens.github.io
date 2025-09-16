---
layout: project
show_home: true

title: Guaraná
title_logo: assets/images/proj-guarana/logo.png
banner_image: assets/images/proj-guarana/gua1.png
banner_style: style7 # 1 to 7

image: assets/images/proj-guarana/card.png
description: Renderize vídeos 360º, vídeos 2D, áudios 3D, objetos 3D, imagens e textos num ambiente imersivo usando um HMD (Head-Mounted Display).

highlights:
  - title: Imersivo
    description: Cria um ambiente sintetizado e interativo para uso com HMDs.
  - title: Segunda Tela
    description: Arquitetura pensada em uso como segunda tela para aplicações DTV.
  - title: Multiusuário
    description: Diferentes usuários podem interagir em um ambiente compartilhado.
  - title: DTV+
    description: Arquitetura integrada à camada de codificação de aplicações da TV 3.0.

spotlight:
  class: custom-right # first element orientation: custom-right, custom-left
  title: Cenas 360 Interativas
  image: assets/images/proj-guarana/guarana360.png
  content: |
    O motor de apresentação Guaraná implementa a API NCL 360 VR da TV 3.0 para renderizar vídeos 360º, vídeos 2D, áudios 3D, objetos 3D, imagens e textos num ambiente imersivo usando um HMD (Head-Mounted Display).
    
    O motor Guaraná está disponível no GitHub.
  urls:
    Código: http://github.com/multisens/guarana2
    Documentação: https://multisens.com.br/TestPages/
---

## Descrição Declarativa

![](/assets/images/proj-guarana/code.png){: .image .left}

A linguagem NCL360 define uma notação simplificada para a criação de uma cena 360 a ser executada no motor de apresentação Guaraná. A notação é baseada na linguagem NCL, permitindo a criação da cena num formato similar aquele usado para a criação de aplicações multimídia interativas.

Assim como em NCL, todo o comportamento da cena é definida indicando as mídias que fazem parte da cena e os *links* que definem quando cada mídia é executada. Diferente da linguagem NCL tradicional, NCL360 posiciona as mídas ao redor do usuário, formando um cenário em 360º.

<br>

## Arquitetura

![](/assets/images/proj-guarana/arquitetura_pt.png){: .image .fit}

A arquitetura do motor Guaraná é definida para possibilitar a integração de tecnologias de VR em apresentações multimídia interativas na TV. A arquitetura proposta se baseia no uso de dispositivos HMD como uma “segunda tela” da aplicação de TV. Desta forma, enquanto a TV apresenta o conteúdo trandicional de uma aplicação, usuários com HMD podem assistir a um formato imersivo como um conteúdo adicional.


## Publicações

| *Joel dos Santos, Rômulo Vieira, Marina Ivanov Josué, Karen Sá Oliveira, Débora Christina Muchaluat Saade*. **Multidevice Support in the Next Generation of the Brazilian Terrestrial TV System**. ACM International Conference on Interactive Media Experiences Workshops (2024) &nbsp; [![download](/assets/images/download.png)](https://dl.acm.org/doi/abs/10.1145/3672406.3672412) |
| *Marcelo F Moreno, Carlos Pernisa Júnior, Eduardo Barrere, Stanley Teixeira, Cristiane Turnes Montezano, Li-Chang Shuen, Carlos de Salles Soares Neto, Débora Christina Muchaluat-Saade, Marina Ivanov Josué, Joel AF dos Santos, Sérgio Colcher, Daniel de S Moares, Derzu Omaia, Tiago Maritan Ugulino de Araújo, Guido Lemos de Souza Filho*. **R&D Progress on TV 3.0 Application Coding Layer**. SET International Journal of Broadcast Engineering (2023) &nbsp; [![download](/assets/images/download.png)](https://revistas.set.org.br/ijbe/article/view/256) |
| *Karen SS Oliveira, Paulo RM de Macedo, Marina IP Josué, Débora C Muchaluat-Saade, Joel AF dos Santos*. **TV 3.0: A Ginga-NCL and Common Core Webservices Extension for Multidevice Support**. Workshop Futuro da TV Digital Interativa (2023) &nbsp; [![download](/assets/images/download.png)](https://sol.sbc.org.br/index.php/webmedia_estendido/article/view/25670) |
| *Gabriel Souza, Daniel Silva, Matheus Delgado, Renato Rodrigues, Paulo RC Mendes, Glauco Fiorott Amorim, Alan LV Guedes, Joel dos Santos*. **Interactive 360-degree videos in ginga-ncl using head-mounted-displays as second screen devices**. Braziliam Symposium on Multimedia and the Web - WebMedia (2020) &nbsp; [![download](/assets/images/download.png)](https://dl.acm.org/doi/abs/10.1145/3428658.3430972) |