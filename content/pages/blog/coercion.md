---
title: Coercion en Javascript
subtitle: Coercion o tipado débil
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
## Tipado debil o fuerte en programacion

Los lenguajes de programación pueden clasificarse según cómo declaramos el tipo de datos que aceptan sus variables. tenemos lenguajes de tipado dinámico o estático y aquellos de tipado fuerte o débil.

Esto se basa **según si permiten o no violaciones de los tipos de datos una vez declarados.**

Los lenguajes de tipado débil son aquellos que realizan las necesarias conversiones de forma interna para hacer un tratado de las variables según la ejecución. Javascript pertenece a este grupo.

**Un tipado blando (o no tipado) significa que las variables son declaradas sin un tipo.**

**Ejemplo:**

var a = 2;

var b = "1";

var c = a - b;

¿Cuanto vale c ?

Respuesta al final del post.

Como ves en javascript  **la declaración de variables no exige la asociación con un tipo de datos de forma implícita.**

Un lenguaje con tipado fuerte seria Java sus variables se declaran así:

private static final Int Name_Var = 2;

La cuarta palabra es Int esto quiere decir que va a aser una variable de tipo numero entero. En este lenguaje se tiene que especificar que tipo de variable es.

## Coerción

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
