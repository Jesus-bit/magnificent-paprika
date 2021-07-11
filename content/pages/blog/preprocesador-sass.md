---
title: Sass el mejor preprocesador
subtitle: Introducción a sass
date: '2021-07-09'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: Un preprocesador en una manera mas fácil de escribir css
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
---
## ¿Por que Sass?

Sass (Syntactically Awesome StyleSheets) es una extensión de CSS que añade características muy potentes y elegantes a este lenguaje de estilos.

Sass es basado en Ruby a diferencia de Less y Stylus que se basan en Javascript.

Sass nos permite usar variables , reglas anidadas , mixins y funciones.

### Facil de aprender

Es como un css pero con mas libertad en la sintaxis y menos lineas de codigo por ejemplo en sass no tienes que colocar llaves ni **punto y coma.**

Esto tiene una excepción por que si tienes tus archivos con extencion ‘.scss’ es porque esta nos permite usar una sintaxis muy parecida a css.

pero si usamos ‘.sass’ la única diferencia es que con esta extensión podremos omitir las llaves ‘{}’ y los punto y coma ‘;’ después de cada valor, esta sintaxis interpretará los atributos y valores por medio de la identación.

#### Sus atributos son:

*   Anidacion: te sirva para escribir mas fácil las clases por ejemplo si tienes una clase .perfil y otra que se llama .perfil\_\_avatar usas & para decirle que perfil estará en las dos clases

*   variables: Sirven para no tener que escribir un color o algun dato que se repita muchas veces los puedes guardar en una variable con el signo de dolar $

*   Extend: si tienes varios elemento que vayan a tener los mismos estilos como un header y un footer puedes utilizarlos por ejemplo si tienes la clase perfil pero un h2 también tendrá los mismos estilos entonces utilizas un @extend de perfil y lo dos tendrán los estilos iguales.

*   Mixins : es parecido a un @extend pero una de las mayores diferencias con los Extends, es que los Mixins pueden recibir argumentos, los cuales te permitirán producir una gran variedad de estilos con unas simples líneas.

#### Reglas de control de flujo

**Sass admite cuatro reglas de control de flujo:**

*   **@if and @else:** Controla si se evalúa o no un bloque

*   **@each:** evalúa un bloque para cada elemento de la lista o par en un mapa.

*   **@for:** evalúa un bloque cierto numero de veces

*   **@while:** evalúa un bloque hasta que se cumpla cierta condición.

Link documentación oficial: <https://sass-lang.com/documentation/at-rules/control>

