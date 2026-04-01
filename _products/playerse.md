---
layout: product
title: "Player NCL"
description: "Player NCL para Efeitos Sensoriais no middleware Ginga."
banner_image: "assets/images/banner.jpeg"
---

O **Player NCL para Efeitos Sensoriais** permite que o *middleware* Ginga dê suporte a aplicações NCL com efeitos sensoriais. Cada efeito é definido como se fosse uma mídia convencional de NCL, sem a necessidade de uso de código adicional.

<ul class="actions" style="margin-top: 2em;">
    <li><a href="https://github.com/GPMM/ginga" class="button special" target="_blank">Ver projeto no GitHub</a></li>
</ul>

---

### Principais Características

* **💻 Extensão da Linguagem:** Estende a linguagem NCL, permitindo a criação de objetos de mídia que representam efeitos sensoriais.
* **📍 Independência de Atuadores:** Os efeitos são definidos de forma independente dos atuadores disponíveis no ambiente, com uso de coordenadas polares para seu posicionamento.
* **📺 Suporte Nativo:** Estende o *middleware* Ginga para suporte direto a efeitos sensoriais.
* **🧩 Arquitetura Flexível:** Permite o uso de diferentes protocolos de comunicação com atuadores de efeitos sensoriais.

---

### Extensão do Middleware

Inclusão de um novo *player* no *middleware* Ginga-NCL para execução de mídias de efeitos sensoriais. Assim, um efeito é definido como uma mídia de NCL, sem necessidade de utilizar código adicional para controlá-la.

<span class="image fit" style="background-color: #ffffff; padding: 20px; border-radius: 8px; max-width: 600px; margin: 0 auto;">
  <img src="https://eic.cefet-rj.br/~gpmm/wp-content/uploads/2020/07/classes.png" alt="Classes de Extensão do Middleware">
</span>

<br>

### Maior Integração

Como o controlador do efeito sensorial faz parte do *middleware* Ginga-NCL, quaisquer alterações de propriedades feitas no documento NCL refletem numa alteração do efeito sendo reproduzido. Tudo transparente para o autor.

<span class="image fit" style="background-color: #ffffff; padding: 20px; border-radius: 8px;">
  <img src="https://eic.cefet-rj.br/~gpmm/wp-content/uploads/2020/07/diag-ginga.png" alt="Diagrama de Integração Ginga">
</span>

<br>

<span class="image fit" style="background-color: #ffffff; padding: 20px; border-radius: 8px;">
  <img src="https://eic.cefet-rj.br/~gpmm/wp-content/uploads/2020/07/timeline-aplicacao.png" alt="Timeline da Aplicação">
</span>