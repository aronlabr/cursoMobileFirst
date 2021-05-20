# Curso de Movil First - Proyecto Batatabit

* [Setup Inicial](#septual-inicial)
* [Diseño Web](#diseño-web)
  * [Header](#header)
  * [Sección 1](#sección-1)
  * [Sección 2](#sección-2)
  * [Sección 3](#sección-3)
  * [Sección 4](#sección-4)
  * [Footer](#footer)
  * [Media Queries](#media-queries)

## Setup Inicial

Cuando tenemos un archivo de figma, este nos genera código CSS recomendado, sin
embargo no debemos utilizarlo y solamente debe servirnos como base para tomar las
medidas y de este código unicamente tomaremos la fuente y los colores.

> El mobile first tiene la ventaja de que es mas fácil añadir elementos al escalar
el documento que eliminarlos, por lo que crear la vista mas simple en primer
lugar facilita la creación de las vistas de mayor dimensión.

Ademas diseñar el sitio mobile-first ayuda a mejorar el SEO de la pagina web.

Es importante realizar la estructura inicial del proyecto en el archivo HTML, es
decir los elementos: header, main, section y footer.

Es importante que todos los nombres de mis archivos deben de ir en minúsculas,
debemos crear una estructura de carpetas similar a la siguiente:

```text
/
├── css/
├── assets/
│   ├── icons/
│   └── img/
└── index.html
```

Cuando escribimos nuestra hoja de estilos es importante tener un orden en el cual
vamos a declarar nuestras reglas de CSS, el orden recomendado es:

1. Posicionamiento: static, absolute, display, etc.
2. Modelo de Caja: margin, border, padding, etc.
3. Tipografías: tipos de letra, tamaños de letra, etc.
4. Estilos visuales: border-radius, shadow, etc.
5. Otros.

Lo primero que vamos a declarar en la hoja de estilos va a ser el elemento `:root`
el cual va a contener todas las variables que vamos a usar en el documento, esto
se hace de esta manera:

```css
:root { /* Cada uno de los colores que se usan en el sitio web */
  --bitcoin-orange: #f7931a;
  --soft-orange: #ffe9d5;
  --secondary-blue: #1a9af7;
  --soft-blue: #e7f5ff;
  --warm-black: #282623;
  --black: #201e1c;
  --grey: #bababa;
  --off-white: #faf8f7;
  --just-white: #fff;
}
```

Si un estilo de fuente es usado en la mayor parte del proyecto lo podemos colocar
en el elemento `html` y sobre-escribir la propiedad en los elementos individuales
cuando sea requerido, es importante no usar una gran cantidad de tipografías, ya
que esto afecta al rendimiento de la pagina, debemos procurar solo traer la menor
cantidad de fuentes y variantes posibles, asi mismo limitar la cantidad de tipos
de fuente a 2.

### Convenciones

Al momento de añadir estilos a los elementos HTML se puede seguir como 
referencia las seguientes convenciones para reducir el tiempo y tener un orden.
1. Posicionamiento --> static, absolute, relative, fixed
2. Modelo de caja (Box model) --> margin, border, padding, content
3. Tipografía --> tipos, tamaños de fuente, etc
4. Estilos visuales --> box-shadow, border-radius, gradient, etc
5. Otros --> reglas CSS y más

[Figma project](https://www.figma.com/file/sMmlQaZldfDcLERYYWe6h4/Bata-Bit?node-id=44%3A593)

### Reniciar estilos de Navegador
Cada navegador tienes diferentes estilos por defecto para las etiquetas HTML lo que hace complicado el proceso de desarrollo, para eso como paso previo: 
```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    font-size: 62.5%; /* Pasar reducir el tamaño del rem = 10px */
}
```

## Diseño Web
### Header
### Sección 1
### Sección 2
### Sección 3
### Sección 4
### Footer
### Media Queries
