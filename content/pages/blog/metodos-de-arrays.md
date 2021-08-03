---
title: Metodos de arrays en javascript
subtitle: 'Como usar short(), map(), filter(), etc.'
date: '2021-08-01'
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
## ¿Que es un array?

Los arreglos son una estructura de datos que tiene la particularidad de disponer de varios datos que se pueden acceder con un mismo nombre.

imagina que tienes una variable llamada  colores y en esta misma almacenamos un color en cada lugar de una caja de colores.

![](/images/code.png)

Cada espacio en una caja de colores representa una posición en nuestro arreglo. **Los arreglos siempre comienzan en la posición 0.**

Entonces red esta en la posición 0 y la ultima posición de este array es 3.

## Métodos

Existen diferentes metodos que estan ya definidos por el lenguaje que nos permiten manipular los arrays. Algunos de estos son:

*   push(). agrega un elemento al final del array.

*   pop().Borra el ultimo elemento del array.

*   unshift(). Agrega un elemento al inicio del array

*   shift(). Borra el primero elemento del array

*   splice(). agrega un elemento en cualquier posición del array.

Los metodos mas avanzados son:

#### map()

El nombre completo de este método es mapeo lo que le hace a un array es transformarlo. map es un callback es decir una función que recibe como parámetro una función, es decir, map() recibe una funciona como parámetro.

el como funciona un map de forma rudimentaria es:

Tienes un array con números del 1 al 5 que son los precios de productos pero se devalúa la moneda tres veces su valor asi que tienes que multiplicar por tres cada numero pero no puede hacerlo uno por uno la solución es sencilla usas un ciclo for de la siguiente forma:

![](/images/caring-saturn.png)

Pues este código hará lo que quieres pero el map() son menos lineas de código y mas efectivo para saber como es que funciones volvamos al ejemplo anterior como tienes que hacer que por cada elemento se multiplique por tres.

El map como parámetro le vas a dar una función y esa función  va a recibir un parámetro este parámetro es cada elemento dentro del array. A este parámetro con una arrow función (es de una sola linea) lo vas a multiplicar por tres, de la siguiente forma:

### ![](/images/code\(3\).png)

### Filter().

Como su nombre lo dice lo que hace es filtrar y filtra en base a una condición que le tienes que dar dentro de una función que le das como callback. lo que hace de manera mas simple es repasar el array y este evalúa una condición que tu le diste como parametro. Así es en código viejo:

![](/images/code\(4\).png)

Para hacerlo con filter básicamente filter te va a dar los valores del array y tu con una función colocas que condición usas para filtrar los elementos del array.

![](/images/code\(5\).png)
