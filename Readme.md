# Curso Practico de Frontend Developer de Platzi

En este curso haremos un proyecto nuevo. Conciste en una venta de garage, este sera responsive y aprenderemos las buenas practicas del desarrrollo web.

Este curso es la continuacion del **Curso de Frontend** Developer de **Platzi**

- [Curso Practico de Frontend Developer de Platzi](#curso-practico-de-frontend-developer-de-platzi)
  - [Sistema de Diseño](#sistema-de-diseño)
    - [Variables CSS](#variables-css)
    - [Fuentes](#fuentes)

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
