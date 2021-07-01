---
title: 'Selectores, Seso y Especificidad en CSS'
subtitle: El peso de los selectores en css
date: '2021-07-01'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
excerpt: la especificidad en css
thumb_image: /images/especificidad.png
image: /images/especificidad.png
---
## Especificidad en selectores

La especificidad es muy importante ya que es el orden por el cual el navegador decide qué estilos aplicarle a un elemento. El orden en cual se decide esto es el siguiente:

1.  Importancia del selector

2.  Especificidad

3.  Orden de las fuentes → Como se mandan a llamar

Si 2 reglas tiene la misma importancia, pasa a evaluarse la especificidad de cada una. Si cuentan con la misma especificidad, pasa el orden a decidir cual se aplica.

En cuestión de importancia, estas son las reglas que primero se aplican:

1.  !important

2.  inline styles

3.  \#ids

4.  .class

5.  tag

Donde a **!important e inline styles** debemos evitarlos las mayorías de veces ya que son mala práctica. Siempre debemos tratar de usar las clases.

En cuanto al orden de las fuentes:

Si se mandan a llamar unos estilos arriba y otros abajo (los dos con la misma clase) los últimos llamados sobrescribirán a los primeros, porque tal como su nombre lo indica, los estilos CSS se leen en cascada y guarda los últimos cambios/valores que lee. (Este es un caso muy extremo)

![](http://tech.tribalyte.eu/wp-content/uploads/2018/09/17.png)

Tomando en cuanta esto ¿cual de los siguientes selectores tiene mas peso?

*   \#id {}

*   .class .classs {}
