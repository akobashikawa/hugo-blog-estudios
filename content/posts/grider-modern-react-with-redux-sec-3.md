---
title: "Modern React with Redux - Sec 3"
subtitle: "Building Content with JSX"
slug: "grider-modern-react-with-redux-sec-3"
summary: ""
featuredImagePreview: "grider-modern-react-with-redux-featured.jpg"
featuredImage: "grider-modern-react-with-redux.jpg"
images: ["grider-modern-react-with-redux.jpg"]
categories: ["Grider - Modern React with Redux"]
tags: ["react", "javascript", "frontend", "udemy"]
author: Antonio Kobashikawa
date: 2022-05-23T21:05:00-05:00
draft: false
---

## Sección 3: Communicating with Props

- Componentes
- Bloque de Comentarios como ejemplo
- **Semantic UI** como biblioteca de estilos
  ```html
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/semantic-ui@2.4.2/dist/semantic.min.css">
  ```
- Extrayendo un bloque repetido como componente
- Utilidad **faker-js** para contenido ficticio
  ```js
  import faker from '@faker-js/faker';
  faker.image.avatar()
  ```
- Componentes anidados
- Props de un componente
  ```jsx
  const CommentDetail = (props) => {
    return (
      <a href="#" className="author">{props.author}</a>
    );
  }
  ```
- Tarjeta de aprobación como ejemplo
- Hijos de componentes
  ```jsx
  <ApprovalCard>
    <CommentDetail
      ...
    />
  </ApprovalCard>
  ```
  ```jsx
  const ApprovalCard = (props) => {
    return (
      <div class="content">
        {props.children}
      </div>
    );
  }
  ```