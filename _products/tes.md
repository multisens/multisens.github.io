---
layout: product
title: "TES"
description: "Tradutor de efeitos sensoriais de NCL para o padrão MPEG-V no middleware Ginga."
banner_image: "assets/images/banner.jpeg"
---

O **TES (Simulador / Tradutor de Efeitos)** traduz informações de efeitos sensoriais especificadas como propriedades de mídias NCL para uma descrição compatível com o padrão MPEG-V. O tradutor, implementado em Lua, é totalmente compatível com o *middleware* Ginga-NCL.

<ul class="actions" style="margin-top: 2em;">
    <li><a href="https://github.com/GPMM/TES" class="button special" target="_blank">Ver projeto no GitHub</a></li>
</ul>

---

### Principais Características

* **📶 Comunicação de Rede:** Traduz uma descrição NCL para o padrão MPEG-V e a envia na rede para um *Media Processing Engine*.
* **💻 Padrão MPEG-V:** O resultado da tradução é um metadado formatado e estritamente compatível com o padrão internacional MPEG-V.
* **📺 Compatível com Ginga:** Pode ser usado em aplicações que rodem nativamente no *middleware* Ginga, sem necessidade de alterações no padrão.

---

### Arquitetura do Tradutor

<span class="image fit" style="background-color: #ffffff; padding: 20px; border-radius: 8px;">
  <img src="https://eic.cefet-rj.br/~gpmm/wp-content/uploads/2020/07/arquit-ncl-mpegv-NOVA.png" alt="Arquitetura do Tradutor NCL para MPEG-V">
</span>