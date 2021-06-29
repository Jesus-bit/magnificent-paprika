---
title: Como funcionan las medidas en css
subtitle: Rem es la mejor medida que puedes utilizar
date: '2021-06-29'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: Usar REM es la mejor practica
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
thumb_image: /images/unnamed.png
image: /images/unnamed.png
---
Medidas absolutas

Su valor se encuentra definido en términos concretos y de manera medible. Esto quiere decir que no depende de otro valor de referencia, ni del contexto.

*   mm: milímetros.

<!---->

*   cm: centímetros.

<!---->

*   in: pulgada (“inches”, en inglés). Una pulgada equivale a 2.54 centímetros.

<!---->

*   pt: puntos. Un punto equivale a 1 /72 de pulgada, es decir, unos 0.35 milímetros.

<!---->

*   pc: picas. Una pica equivale a 12 puntos, o aproximadamente a 4.23 milímetros.

<!---->

*   px: pixel. Es la unidad mínima de resolución de la pantalla. En realidad suele considerársela una unidad absoluta, relativa o híbrida dependiendo del criterio que se analice.

Si analizamos que el pixel es una división física de la pantalla podríamos decir que corresponde definirla como unidad absoluta. Sin embargo, en los diferentes dispositivos estos pixeles tienen variaciones de tamaño, que aunque son mínimas y a veces imperceptibles, dan pie a que algunos autores la consideren unidad relativa.

La principal ventaja de las unidades absolutas es que su valor es el que está expresado y el que se va a aplicar, no hay que hacer cálculos intermedios. Sin embargo, a pesar de esta aparente ventaja, no son las más utilizadas ya que resultan poco adaptables a la multiplicidad de dispositivos.

Unidades relativas

Las unidades relativas no son valores exactos sino que se calculan a partir de otro valor de referencia. A pesar de parecer más difíciles de calcular son las más utilizadas en el diseño de sitios web responsive por su adaptabilidad a los diferentes dispositivos.

*   Porcentaje (%), es una de las unidades relativas más utilizadas. Su valor está calculado siempre en base a otro elemento. Si lo aplicamos sobre una fuente es relativo al tamaño de la fuente declarada en el contexto, pero si lo aplicamos al width de un elemento entonces es relativo al ancho de su contenedor.

Unidades relativas a la tipografía

*   em: unidad relativa al tamaño de texto definido en un determinado contexto. El em hace referencia al tamaño de letra que se está usando.

Cuando se utiliza la unidad em, es imprescindible conocer el valor de referencia, de lo contrario saber que un texto tiene 1em ó 5em no nos dice realmente el tamaño de la letra.

Cuando se asigna una medida en ems, su referencia es el tamaño de letra del primer elemento contenedor que tenga establecido un tamaño de letra.

\<article>

\<h2> Título \</h2>

\<p> Texto del párrafo \</p>

\</article>

article {

font-size: 20px;

}

h2 {

font-size: 1.5em;

}

p {

font-size: 0.9em;

}

El font-size de 18px definido en el article, lo convierte en el valor de referencia para calcular la medida del h2 y del p. En este caso el \<h2> equivale a 30px, y el \<p> mide 18px.

Si este elemento no se encuentra contenido en ningún otro, entonces la referencia es el tamaño de letra establecido en el \<body>. Por último, en el caso de que no haya definido un font-size en el body, entonces se toma el valor por defecto establecido por los navegadores. La mayoría de los navegadores define el tamaño de los párrafos en 16px, el valor del em entonces será equivalente a 16 px. En tal caso, si indicara que el line-height sea de 1.5em, estaría diciendo que mida 24px.

*   ex: unidad relativa a la altura de la letra “x” minúscula de un determinado cuerpo y alfabeto. También es un concepto proveniente del diseño tipográfico.

<!---->

*   rem: funciona igual que el em, con la diferencia que es relativo al valor de la fuente del elemento html, y no tiene en cuenta el valor heredado o del elemento que lo contiene.

## MEDIDA REM

REM : funciona igual que el em, con la diferencia que es relativo al valor de la fuente del elemento html, y no tiene en cuenta el valor heredado o del elemento que lo contiene.

Por defecto el html viene con un tamaño de fuente de 16px asi que siempre

1 REM = 16PX

Si queremos aplicar rem de una forma mas sencilla para no tener que hacer tantos calculos asemos lo siguiente

html {
	font-size: 62.5%;
}

esto lo que hara es darle a el html un valor de 10px ya que 16px - 62.5% = 10px

ahora si por ejemplo a una etiqueta le asignamos 2rem este hara referencia a 20px, o si por ejemplo le damos un valor de 1.5rem su valor sera de 15px

la estructura que siempre debe llevar tus archivos de css es

html {
font-size: 62.5%
}
