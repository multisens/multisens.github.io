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
    description: Pensado para uso em HMDs (Head-Mounted Displays). Cria um ambiente sintetizado e interativo.
  - title: Segunda Tela
    description: Arquitetura pensada em uso como segunda tela para aplicações de TV digital.
  - title: Multiusuário
    description: Cada usuário em seu HMD compartilha um mesmo ambiente com os demais.
  - title: Compatível com SBTVD
    description: Arquitetura integrada ao middleware Ginga do Sistema Brasileiro de TV Digital.

spotlight:
  class: custom-right # first element orientation: custom-right, custom-left
  title: Cenas 360 Interativas
  image: assets/images/proj-guarana/guarana360.png
  content: Renderize vídeos 360º, vídeos 2D, áudios 3D, objetos 3D, imagens e textos num ambiente imersivo usando um HMD (Head-Mounted Display).
  urls:
    GitHub: http://github.com/multisens/guarana2
---

# Descrição Declarativa

![](/assets/images/proj-guarana/code.png){: .image .left}

O formato NCL360 utilizado pelo player Guaraná permite a criação simplificada da cena 360 a serem executadas. O formato é baseado na linguagem NCL, permitindo a criação da cena num formato similar aquele usado para a criação de aplicações multimídia interativas.

<br><br><br><br><br>

# Arquitetura

{% include canvas.html src="assets/images/proj-guarana/arquitetura_pt.png" height="270px" %}

Arquitetura definida para possibilitar a integração de tecnologias de VR em apresentações multimídia interativas na TV. A arquitetura proposta se baseia no uso de dispositivos HMD como uma “segunda tela” da aplicação de TV. Desta forma, enquanto a TV apresenta o conteúdo trandicional de uma aplicação, usuários com HMD podem assistir a um formato imersivo como um conteúdo adicional.