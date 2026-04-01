---
layout: product
title: "MBook"
description: "Plataforma de leitura multissensorial imersiva com rastreamento ocular."
banner_image: "assets/images/banner.jpeg"
---

O **MBook** permite que você se sinta dentro do ambiente narrado no livro, experimentando efeitos sensoriais perfeitamente sincronizados com a leitura. O objetivo principal do projeto é estimular a leitura, criando um ambiente altamente imersivo e divertido para o usuário.

<ul class="actions" style="margin-top: 2em;">
    <li><a href="https://github.com/GPMM/mbook" class="button special" target="_blank">Ver projeto no GitHub</a></li>
</ul>

---

### Principais Características

* **👀 Eye-Tracker:** Acompanha a leitura do usuário em tempo real utilizando um rastreador ocular, permitindo que os eventos do livro sejam acionados pela velocidade e posição de leitura de cada pessoa.
* **🌬️ Multissensorial:** Utiliza atuadores no ambiente físico para reproduzir efeitos de vento, cheiro, iluminação, vibração, sons e muito mais, complementando a narrativa.
* **📄 Descrição Declarativa:** Utiliza o formato XML para descrever a lógica de criação do cenário multissensorial e a estrutura textual do livro, mantendo a narrativa desacoplada dos detalhes de implementação técnica dos atuadores.

---

### Arquitetura do Sistema

A arquitetura do MBook é desenhada para ser modular e é composta de três componentes principais:

1. **Biblioteca:** O repositório que contém os livros já carregados no sistema e prontos para serem lidos.
2. **Leitor:** O motor principal que recebe a informação textual do livro junto com a lógica da cena multissensorial. Ele exibe o conteúdo e ativa os efeitos de acordo com o avanço da posição de leitura.
3. **Controlador:** O módulo responsável por fazer a interface direta com os dispositivos e atuadores físicos disponíveis no ambiente onde a leitura ocorre.

<span class="image fit" style="background-color: #ffffff; padding: 20px; border-radius: 8px;">
  <img src="https://eic.cefet-rj.br/~gpmm/wp-content/uploads/2020/07/arquitetura_pt-1.png" alt="Arquitetura do MBook">
</span>