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

\-var: puede ser re declarada y reasignada

\-const: No puede ser re declarada ni reasignada

\-let: Puede ser reasignada pero no re declarada.

El scope que tiene cada forma de declarar variables es diferente. los tipos de scope son:

\-Global: Cuando una variable esta en este scope desde cualquier función o lugar del programa puede ser consultada.

\-function: En este scope la variable solo puede ser consultada dentro de la función en la cual fue declarada

\-Block: la variable solo esta disponible en un bloque que este entre llaves { } como un bucle.

