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

El scope es el alcance que tienen las variables, es decir, en que parte del código pueden ser consultadas o modificadas las variables. Inicializacion y declaración de variables no es lo mismo, cuando tu declaras una variable sin inicializar su valor es undefindied y puedes re-asignar una variable en ciertos casos, es decir cambiarle su valor. En javascript hay tres maneras de declarar variables con:

\-var: puede ser re declarada y reasignada

\-const: No puede ser re declarada ni reasignada

\-let: Puede ser reasignada pero no re declarada.
