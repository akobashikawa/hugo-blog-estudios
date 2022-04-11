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
date: 2022-04-10T12:09:00-05:00
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

### Class
- Las clases permiten agrupar variables y métodos relativos a una entidad.
- Con la **herencia** una clase puede tener ciertas variables y métodos de una clase base.
  - Se usa `extends`
- **class** Animal
	- **constructor()**
		- **this**.x
- new Animal()
- class Lion **extends** Animal
	- constructor()
		- **super()**
- new Lion()

{{< admonition note "Sobre las clases en javascript" >}}
- En javascript, propiamente, **no existen las clases sino sólamente objetos**.
  - La herencia se realiza mediante **prototipos**.
- El uso de clases son un agregado (*sugar code*), realizado gracias a los **transpiladores**, para que los desarrolladores que vienen del mundo OOP se sientan más cómodos.
- He leído que usar prototipos para herencia en lugar de clases puede facilitar algunas cosas y que **es importante no olvidar** que existe esa opción en javascript.
{{< /admonition >}}

### State
- this.**state** = { stateName: value }
- this.**setState**({ stateName: value })
	- En react, **no es una buena práctica modificar directamente el estado** stateName, sino usando setState()
	- La razón es que **una modificación directa tiene que esperar hasta que se ejecute render()** para que se vea reflejado el cambio.
		- Mientras que **setState() se asegura de ejecutar render()** inmediatamente después de la modificación.
- **onClick**={this.handlerMethodName}
	- En javascript, **una función se puede pasar como argumento**, igual que como se hace con otras variables.
		- No es como en otros lenguajes, donde se necesitaría usar una referencia a su posición en memoria.

### Binding
- Cuando se define un método, su variable **this** coge el **contexto** en curso.
- Los métodos definidos de la manera tradicional no tienen el contexto del componente y hay que agregarlo explícitamente.
	- this.myMethod() { console.log(this); // undefined }
- Una forma de que tuvieran el contexto del componente sería **definirlos dentro de su constructor**.
	- Pero **no sería muy legible**.
- Otra forma de que tengan el contexto del componente es **definirlos fuera del constructor**, por legibilidad, pero **actualizar sus contextos en el constructor**.
	- this.myMethod = this.myMethod.**bind(this)**
- Otra forma de que tengan el contexto del componente es **definirlos como una función arrow**, que sí toma el contexto del componente.
	- this.myMethod = () **=>** { console.log(this); // ok }

### Globals
- Las **variables globales** se nombran en mayúsculas, siguiendo la convención **SCREAM_UPPERCASE**.

### Props
- Se pueden pasar propiedades a un componente a través de los atributos de su etiqueta.
	- `<Project project={PROJECT} />`
	- En el componente Project se ve a través de **this.props**.project 