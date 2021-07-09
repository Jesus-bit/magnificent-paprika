---
title: Scroll horizontall con css
subtitle: mejor practica de mobile first
date: '2021-07-08'
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
thumb_image: /images/images.png
---
#### ¿Por que un Scroll horizontal es bueno?

Cuando trabajar responsive desing lo que queremos es que el usuario tenga una buena experiencia desde un dispositivo mobile asi que cuando tengamos una serie de elementos que crean un overflow lo mejor es que en lugar de que toda la pantalla se tenga que deslizar hacia un lado. solo se deslize el contenedor 



![](https://francescricart.com/wp-content/uploads/2018/12/resumen-propiedad-overflow-css.jpg)

para mejorar este posicionamiento es con las siguientes propiedades: 

[overflow-x](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-x)

La propiedad de CSS overflow-x establece lo que se muestra cuando el contenido desborda los bordes izquierdo y derecho de un elemento a nivel de bloque. Puede que no sea nada, una barra de desplazamiento o el contenido adicional.

[overscroll-behavior](https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior)

la propiedad de css overscroll-behabior establece lo que hace un navegador cuando alcanza el límite de un área de desplazamiento. Es una abreviatura de overscroll-behavior-x y overscroll-behavior-y.

[scroll-snap-type](https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-snap-type)

La propiedad CSS scroll-snap-type establece qué tan estrictamente se aplican los puntos de snap en el contenedor de desplazamiento en caso de que haya uno
