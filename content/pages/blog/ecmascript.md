---
title: ECMAScript 6 +
subtitle: Ecmascript es el estándar de Javascript.
date: '2021-08-11'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: El estándar en javascript
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
thumb_image: /images/1da09a35-1e5c-4aef-9317-e88f2cb445d1.png
image: /images/1da09a35-1e5c-4aef-9317-e88f2cb445d1.png
---
## ¿Que es ECMAScript?

**ECMAScript** es la especificación del lenguaje propuestro por **ECMA** Internacional que es una institucíon encargada de los estándares, y JavaScript es el lenguaje de programación que utiliza esta especificación para trabajar sobre estas características que van siendo añadidas año con año desde el 2015.

Cada junio de cada año, y esto es mediante una propuesta, y un comité encargado de revisar estas características que se añadirán al lenguaje.

Lo mas relevante desde el ECMAScript 6 es:

## Arrow Functions y Promesas

**Arrow Functions:  =>**

const helloPromise = () => {
return new Promise((resolve, reject)=>{
if(false){
resolve('Hello!');
} else{
reject('Woops!!');
}
});
}

helloPromise()
.then(response => console.log(response))
.catch(error => console.log(error));
