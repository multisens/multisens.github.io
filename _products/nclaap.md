---
layout: product
title: "NCLAAP"
description: "Processador de Âncoras Abstratas integrado com redes neurais."
banner_image: "assets/images/banner.jpeg"
---

O **Processador de Âncoras Abstratas (NCLAAP)** permite que o autor de uma aplicação multimídia interativa defina com qual elemento quer sincronizar parte de sua aplicação, sem precisar especificar o momento exato em que ele aparece no vídeo ou áudio. 

Uma âncora abstrata representa um determinado elemento que pode ser visto ou ouvido (por exemplo, uma flor, um som de trovão, etc.). Uma vez definidos os elementos de interesse, o processador descobre os momentos em que eles aparecem e completa a especificação da aplicação multimídia.

<ul class="actions" style="margin-top: 2em;">
    <li><a href="https://github.com/GPMM/Abstract-Anchor" class="button special" target="_blank">Ver projeto no GitHub</a></li>
</ul>

---

### Principais Características

* **🧩 Extensível:** Arquitetura pensada para permitir o uso em conjunto com uma ou mais redes neurais, sem precisar alterar o processador.
* **⚙️ Autoria Simplificada:** Edite uma vez, reprocesse quantas vezes forem necessárias.
* **📺 Compatível com Ginga:** Pode ser usado em aplicações que rodem no *middleware* Ginga da TV Digital, sem necessidade de alterações no padrão NCL.

---

### Integração com Redes Neurais

O Processador usa redes neurais para identificar automaticamente quando determinados elementos aparecem em um vídeo ou áudio. Essa informação é utilizada para criar a temporização das âncoras reais de NCL durante o processamento.

<span class="image fit" style="background-color: #ffffff; padding: 20px; border-radius: 8px;">
  <img src="https://eic.cefet-rj.br/~gpmm/wp-content/uploads/2020/07/AAP_architecture.png" alt="Arquitetura do Processador AAP">
</span>

<br>

### Múltiplos Resultados

Mudou a ordem das cenas? Editou o vídeo? Não tem problema. Basta usar o processador novamente na nova mídia para gerar anotações de tempo atualizadas de forma automática.

<span class="image fit" style="background-color: #ffffff; padding: 20px; border-radius: 8px;">
  <img src="https://eic.cefet-rj.br/~gpmm/wp-content/uploads/2020/07/timeline_tags.png" alt="Timeline Tags">
</span>