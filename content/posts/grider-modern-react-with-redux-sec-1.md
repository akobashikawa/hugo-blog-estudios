---
title: "Modern React with Redux - Sec 1"
subtitle: "Let's Dive In!"
slug: "grider-modern-react-with-redux-sec-1"
summary: "Setup, First App, First React Project, Functional Components"
featuredImagePreview: "grider-modern-react-with-redux-featured.jpg"
featuredImage: "grider-modern-react-with-redux.jpg"
images: ["grider-modern-react-with-redux.jpg"]
categories: ["Grider - Modern React with Redux"]
tags: ["react", "javascript", "frontend", "udemy"]
author: Antonio Kobashikawa
date: 2022-05-23T20:36:00-05:00
draft: false
---

## Sección 1: Let's Dive In!

- Vista general del curso
  - Cómo buscar ayuda 
  - Enlace a la comunidad
- Una primera app usando [CodeSandbox](https://codesandbox.io/) 
- Setup
  - NodeJS
  - Create React App (CRA)
- El sistema de módulos de javascript
- Componentes funcionales

{{< admonition note "Vite en lugar de CRA" >}}
- En el curso se usa CRA, pero yo estoy siguiéndolo con Vite.
- [Create React App](https://create-react-app.dev/) (CRA) es la herramienta oficial, desarrollada por los desarrolladores de Facebook.
  - Tarda varios minutos para empezar cada proyecto
  - Tarda bastante para hacer los rebuilds
- Evan You, creador de VueJS, desarrolló [Vite](https://vitejs.dev/guide/#scaffolding-your-first-vite-project) para facilitar el building de aplicaciones web JS.
  - No está limitado a Vue o React, es más universal.
  - Tiene grandes ventajas de performance sobre CRA.
    - Se empieza un proyecto en menos de un minuto.
      - $ npm create vite@latest
    - El Hot Reloading Module (HRM) es prácticamente instatáneo.    
  - El esquema de trabajo es bastante similar, haciendo algunas adaptaciones menores.
    
    ```html
    <!-- index.html -->
    <script type="module" src="/src/main.jsx"></script>
    ```

    - Se usa jsx para indicar explícitamente que es un archivo jsx.
    - $ npm run dev

{{< /admonition >}}
