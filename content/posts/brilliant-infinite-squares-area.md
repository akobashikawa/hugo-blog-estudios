---
title: "Brilliant - Área de infinitos cuadrados"
subtitle: "¿Puedes medir infinitas áreas?"
slug: "brilliant-infinite-squares-area"
summary: "¿Puedes medir infinitas áreas?"
featuredImagePreview: "brilliant-infinite-squares-area.png"
featuredImage: "brilliant-infinite-squares-area.png"
images: ["brilliant-infinite-squares-area.png"]
categories: ["Matematicas"]
tags: ["matematicas", "brilliant"]
author: Antonio Kobashikawa
date: 2022-04-09T15:38:00-05:00
math:
  enable: true
draft: false
---

## ¿Qué fracción del área mayor será el área en rojo?

Hoy recibí por email este problema de Brilliant.

¿Cual crees que es la respuesta? ¿1/5?, ¿1/4?, ¿1/3?, ¿1/2?, ¿1?

{{< admonition type=note title="Método 1" open=false >}}
  - Para resolverlo recordé un método que aprendí cuando postulaba a la universidad.
  - Si el área total es 1, el área en rojo es R:
    $$ R = \frac{1}{4} + \frac{1}{4}\Big(\frac{1}{4}\Bigr) + \frac{1}{4}\Big(\frac{1}{4}\Bigr)\Big(\frac{1}{4}\Bigr) + ... $$
    $$ \implies 4R = 1 + \frac{1}{4} + \frac{1}{4}\Big(\frac{1}{4}\Bigr) + ... $$
    $$ \implies 4R = 1 + R $$
    $$ \implies R = \frac{1}{3} $$
{{< /admonition >}}

{{< admonition type=tip title="Método 2" open=false >}}
  ![](brilliant-infinite-squares-area-solving.png)
  - Podemos ver que en la L invertida del cuadrado más grande, el area en rojo es 1/3 de esa L invertida
  - Lo mismo es el cuadrado siguiente. El área en rojo es 1/3 de la L invertida de ese cuadrado.
  - Y así, sucesivamente, en cada siguiente cuadrado  el área en rojo es 1/3 de la L invertida de ese cuadrado.
  - Si el área total es 1, el área en rojo es R:
    $$ R = \frac{1}{3}L_1 + \frac{1}{3}L_2 + \frac{1}{3}L_3 + ... $$
    $$ \implies R = \frac{1}{3}(L_1 + L_2 + L_3 + ...) $$
    $$ \implies R = \frac{1}{3}(1) $$
    $$ \implies R = \frac{1}{3} $$
{{< /admonition >}}

## Brilliant

[Brilliant](https://brilliant.org/) es un portal que ayuda a aprender y comprender las matemáticas de manera visual.

{{< youtube xdojCKmLtow >}}