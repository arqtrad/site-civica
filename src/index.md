---
title: "Arquitetura cívica tradicional luso-brasileira"
description: >
  Documentário da arquitetura cívica publicada na bibliografia de 
  referência
layout: "layouts/splash.njk"
lang: "pt-PT"
classes:
  - "splash"
  - "wide"
header:
  teaser       : "https://tradicional.arq.br/media/an-teaser.jpg"
  overlay_image: "https://i.pinimg.com/originals/f8/3e/fb/f83efb2810cb7ae3e05ca3a47afbf7ee.jpg"
  overlay_filter: 0.5
  caption: "Antiga sede do Arquivo Nacional à praça da República, 1905"
triptych:
  - image_path: https://placehold.co/210x210/png
    title     : "Monumentalidade"
    excerpt   : "Um resumo aqui"
    url       : /monumentalidade/
    btn_class : "btn-primary"
  - image_path: https://placehold.co/210x210/png
    title     : "Neocolonial"
    excerpt   : "Transposição de motivos religiosos para a arquitetura cívica neocolonial"
    url       : /neocolonial/
    btn_class : "btn-primary"
  - image_path: https://placehold.co/210x210/png
    title     : "Projetos ideais"
    excerpt   : "Obras cívicas não realizadas"
    url       : /ideal/
    btn_class : "btn-primary"
templateEngineOverride: njk,md
---

# Coleções especiais # {.wide}

::: text-center
Em breve.
:::

```{=html}
{# {% include "partials/triptych.njk" %} #}
````

# {{ schemata.ui_text[locale].recent_posts }} # {.mb-4 .wide}

```{=html}
<div class="row row-cols-md-2 row-cols-xl-3 g-3 mx-5">
{% for post in collections.w | reverse %}
  {% if loop.index0 < 6 %}
    {% include "partials/card-place.njk" %}
  {% endif %}
{% endfor %}
</div>
<div class="d-flex flex-columns row-cols-md-2 row-cols-lg-3 mx-auto mt-4 justify-content-center">
  <a type="button" href="/w/" class="btn btn-outline-primary btn-lg">
    {{ schemata.ui_text[locale].load_all }}
  </a>
</div>
````
