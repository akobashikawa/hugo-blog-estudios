---
title: "React JS - The Essentials Bootcamp - Sec 2"
subtitle: "Welcome to React"
slug: "katz-react-js-the-essentials-bootcamp-sec-2"
summary: "Welcome to React | First React Application"
featuredImagePreview: "katz-reactjs-bootcamp-featured.jpg"
featuredImage: "katz-reactjs-bootcamp.jpg"
images: ["katz-reactjs-bootcamp.jpg"]
categories: ["Katz - ReactJS Bootcamp"]
tags: ["react", "javascript", "frontend"]
author: Antonio Kobashikawa
date: 2022-04-07T12:59:00-05:00
draft: false
---

## Sección 2: Welcome to React | First React Application

- Vista general de la sección 2
  - Sobre la primera aplicación que se construirá
    - Portfolio

### Base
- create-react-app permite crear rápidamente una aplicación react
  - ahora se ejecuta vía npx
- **npx** --version
- npx **create-react-app** portfolio
- src/**index.js**
	- **import** x from 'module'
	- **React**
	- **ReactDOM**
	- ReactDOM.**render()**
		- `#root` @ public/**index.html**
- npm run start
- http://localhost:3000

### Components
- Los componentes son como bloques de lego que se ensamblan para construir la aplicación
- import App from './App'
- App
	- import { **Component** } from 'react'
	- App **extends** Component
	- App.render()
		- return **JSX**
	- **export** default App

{{< admonition note "Sobre los módulos en javascript" >}}
- Javascript no poseía un sistema de módulos hasta hace poco.
- El uso de módulos se lograba con ayuda de transpiladores.
- El soporte actual de módulos permite hacerlo también sin transpiladores.
- Se siguen usando transpiladores por algunas otras tareas que permiten hacer.
  - Como la preparación de un bundle optimizado
- Hay programadores que señalan que el uso de transpiladores agrega una capa más de dificultad al momento de depurar código.
{{< /admonition >}}

### Classes
- Las clases permiten agrupar variables y métodos relativos a una entidad.
- Con la **herencia** una clase puede tener ciertas variables y métodos de una clase base.
  - Se usa `extends`

{{< admonition note "Sobre las clases en javascript" >}}
- En javascript, propiamente, **no existen las clases sino sólamente objetos**.
  - La herencia se realiza mediante **prototipos**.
- El uso de clases son un agregado (*sugar code*), realizado gracias a los **transpiladores**, para que los desarrolladores que vienen del mundo OOP se sientan más cómodos.
- He leído que usar prototipos para herencia en lugar de clases puede facilitar algunas cosas y que **es importante no olvidar** que existe esa opción en javascript.
{{< /admonition >}}