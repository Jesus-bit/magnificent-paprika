---
title: Coercion en Javascript
subtitle: Cambiar de un tipo de valor a otro
date: '2021-07-26'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: lorem-ipsum
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
---
La coerción es la conversión automática o implicita de valores de un tipo de dato a otro (Ejemplo: de cadena de texto a número).

Los dos tipos de coercion se describirian asi:

1.  Coerción implícita: Es cuando el lenguaje nos ayuda a cambiar el tipo de valor.

2.  Coerción explicita: Es cuando obligamos a que cambie el tipo de valor.

### Ejemplos

Coercion implicita

4 + "7";  =   /\* 47 \*/

Lo que pasa aquí es que el signo "+" significa una concatenación y como no es posible unir dos valores de diferente tipo lo que hace javascript es convertir el numero cuatro a string para que el resultado sea "47" un string

4 \* "7";  =   /\* 28 \*/

Coerción explicita

String(10);
Number("10");
ParseInt("10");

Las funciones Number(); y ParseInt(); las tiene por defecto javascript y se usan para convertir valores intencionalmente es decir tu colocas estas funciones específicamente para cambiar el tipo de valor que le des. 
