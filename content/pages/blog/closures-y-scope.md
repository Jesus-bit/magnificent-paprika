---
title: Closures y scope en javascript
subtitle: El alcance de las variables
date: '2021-08-05'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: Una funcion que recibe otra = Callback
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
---
### ¿Que es el scope?

El scope es el alcance que tienen las variables, es decir, en que parte del código pueden ser consultadas o modificadas las variables. Inicializacion y declaración de variables no es lo mismo, cuando tu declaras una variable sin inicializar su valor es undefindied y puedes re-asignar una variable en ciertos casos, es decir cambiarle su valor.

![](/images/code\(1.png)

En javascript hay tres maneras de declarar variables con:

*   var: puede ser re declarada y reasignada

<!---->

*   const: No puede ser re declarada ni reasignada

<!---->

*   let: Puede ser reasignada pero no re declarada.

El scope que tiene cada forma de declarar variables es diferente. los tipos de scope son:

*   Global: Cuando una variable esta en este scope desde cualquier función o lugar del programa puede ser consultada.

<!---->

*   Local: En este scope la variable solo puede ser consultada dentro de la función en la cual fue declarada

<!---->

*   Block: la variable solo esta disponible en un bloque que este entre llaves { } como un bucle.

El global scope es especial pues para que una variable sea global hay dos formas una es declarándola en la raíz del programa, es decir, fuera de cualquier función o llaves. La otra es cunado este declarada dentro de una función y hacerla global seria declararla con la palabra "globalThis"

Bueno para resumir y decirles cual el scope que tiene cada palabra reservada al declarar una variable es con una tabla:

![](/images/const-vs-let-vs-var.png)

### Ejercicio

¿Que mostrara la consola? Respuesta al final de post.

![](/images/code\(7.png)

### ¿Que es un closure?

Juntamos el scope y lo mezclamos con una funcion podemos crear algo llamado closure. un closure es una función interna que tiene acceso al alcance de su funcion externa.

