# Curso Practico de Frontend Developer de Platzi

En este curso haremos un proyecto nuevo. Conciste en una venta de garage, este sera responsive y aprenderemos las buenas practicas del desarrrollo web.

Este curso es la continuacion del **Curso de Frontend** Developer de **Platzi**

- [Curso Practico de Frontend Developer de Platzi](#curso-practico-de-frontend-developer-de-platzi)
  - [Sistema de Diseño](#sistema-de-diseño)
    - [Variables CSS](#variables-css)
    - [Fuentes](#fuentes)
  - [Proyecto Yard Sale](#proyecto-yard-sale)
    - [Contraseña](#contraseña)

## Sistema de Diseño

El sistema de diseño es importante a la hora de iniciar un nuevo proyecto, debido a que en este estableceremos todos nuestros colores, fuentes, logos, etc y de esta manera seremos mas eficientes. Parte de los sistemas de diseño se encuentran:

### Variables CSS

Las variables en *CSS* son muy utiles, con ellas estableceremos un valor para usarlo de forma global, en caso de querer modificarlo, solo bastaria con modificar la variable y este cambio se vera reflejado en todo nuestro codigo a diferencia de tener que modificar nuestros valores linea por linea

Para usar las variables debemos hacer este codigo en nuestra hoja de estilo:

```css
:root {
   --white: #ffffff;
   --black: #000000;
   --very-light-pink: #c7c7c7;
   --text-input-field: #f7f7f7;
   --hospital-green: #acd9b2;
}
```

y listo, para ponerlos en nuestros selectores es del siguiente modo:

```css
propiedad: var(--nombre-variable);
```

### Fuentes

Las fuentes son algo basico en el diseño en general. En este caso usamos [Google Fonts](https://fonts.google.com/) donde podremos buscar la fuente que queramos o nos hallan asignado al proyecto.

Cuando la tengamos, el propio *Google Fonts* nos dara las instrucciones de como enlazarlas a nuestro proyecto, generalmente es asi:

> HTML:

```html
<head>
   <meta charset="utf-8">

   <link rel="preconnect" href="https://fonts.googleapis.com">
   <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
   <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@300;500;700&display=swap" rel="stylesheet">

   <title>Document</title>
</head>
```

> CSS

```CSS
body {
   font-family: "Quicksand", sans-serif;
}
```

Y de este modo tendremos la fuente instalada

## Proyecto Yard Sale

Alfin iniciamos con nuestro proyecto, algo importantisimo y que es muy urgente aclarar es que como se lleva el curso, que es para desarrolladores no muy avanzados, se ven malas practicas, como tener usar estilos dentro de html, hacer la maquetacion Web First y no Mobile First que es la recomenda, entre otras cosas que pueden desencajar lo aprendido anteriormente, vale? por ello me he tomado la mas que justificada libertad de hacer ciertos cambios en el codigo tratando de solucionar algunos de estos fallos

### Contraseña

 arrancamos con la pagina de creacion de contraseña, usamos variables, fuentes, logos, grid y flexbox.

 Algo que aprendi con grid (ya que nunca lo habia usado) fue que con una sola linea de codigo puedas centrar tu contenido, de esta forma:

```css
div {
   display: grid;
   place-items: center;
}
```

Una forma distinta a la usada con flexbox.

Aparte de esto vimos un pequeño truco, si se eliminan los ``margin`` del `body` nuestras medidas relativas de `vw` y ``vh`` no tendran incovenientes para mostrarse ni aparecera la barra de scroll que le hace dar una apariencia no tan pulida a nuestra pagina
