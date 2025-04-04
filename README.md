# Astro Starter Kit: Minimal

```
npm create astro@latest -- --Plantilla mínima
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/minimal)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/minimal)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/minimal/devcontainer.json)

## 🚀 Estructura del proyecto

Dentro de tu proyecto Astro, verás las siguientes carpetas y archivos:

```
/
├── public/
├── src/
│   └── Components/
│       └── footer
│       └── header
│       └── main
│   └── const/
│       └── const.js
│   └── icons/
│   └── pages/
│       └── index.astro
│   └── style/
└── .gitignore
└── README.md
└── astro.config.mjs
└── package-lock.json
└── package.json
└── tsconfig.json
```

Astro busca archivos '.astro' o '.md' en el directorio 'src/pages/'. Cada página se expone como una ruta en función de su nombre de archivo.

En 'src/components/' es donde se utiliza cualquier componente de Astro/React/Vue/Svelte/Preact.

Cualquier activo estático, como imágenes, se puede colocar en el directorio 'public/'.

## 🧞 Comandos

Todos los comandos se ejecutan desde la raíz del proyecto, desde un terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:3000`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |


# Guía de proyecto - Portafolio

# Guía del Código de la Página Principal en `src/pages/index.astro`

Este archivo es la página principal del portafolio de Franklin Pezo, desarrollado con **Astro**. A continuación, se describe la estructura y función de cada parte del código para que puedas entender cómo está organizada la página y cómo puedes personalizarla según tus necesidades.

## Estructura del Archivo

El archivo `index.astro` tiene una estructura sencilla y clara, dividida en varias secciones clave:

1. **Importación de Componentes**
2. **Metadatos de la Página**
3. **Cuerpo HTML**
4. **Descripción de los Componentes**

---

## 1. **Importación de Componentes y Estilos**

```astro
import Header from "../components/header/Header.astro";
import "../style/index.css";
import Main from "../components/main/main.astro";
import Footer from "../components/footer/Footer.astro";
```

## Función de Cada Parte del Código

### Header
Este componente probablemente contiene elementos de navegación como:

- **Logo**.
- **Menú de enlaces** a secciones del portafolio o información de contacto.
- **Información personal** o un saludo.

### Main
Este componente es el núcleo del portafolio, y podría contener secciones como:

- Una **breve descripción** sobre Franklin Pezo Montesinos.
- **Detalles de sus proyectos**.
- **Habilidades y experiencia**.

### Footer
El componente de pie de página podría incluir:

- **Derechos de autor**.
- **Enlaces a redes sociales** (por ejemplo, LinkedIn, GitHub).
- **Información de contacto** o links importantes.

# Guía del Código del Footer `src/components/footer`

## Descripción General

El siguiente código corresponde a la sección del **footer** (pie de página) de una página web. En esta sección se incluyen enlaces a redes sociales y datos de contacto, con un diseño responsivo y atractivo gracias a las propiedades de CSS. La estructura se divide en tres partes principales: el contenido de contacto, los iconos de las redes sociales y el estilo visual.

---

## Estructura HTML

```html
<footer>
  <section class="section-footer">
    <div class="linear-grandient-1"></div>
    <div class="container-footer">
      <h2 class="title-contact" id="contacto">Contacto</h2>
      <div class="container-redes">
        <a href="https://wa.me/( Ingresa tu numero telefónico ) " target="_blank">
          <li class="li-contact">
            <i class="fa-brands fa-whatsapp icon-whatsapp"></i>
            <p>Whatsapp</p>
          </li>
        </a>

        <a href="( Ingresa la URL de tu pagina de Github ) " target="_blank">
          <li class="li-contact">
            <i class="fa-brands fa-github"></i>
            <p>Github</p>
          </li>
        </a>

        <a
          href="( Ingresa la URL de tu pagina de Linkedin )"
          target="_blank"
        >
          <li class="li-contact">
            <i class="fa-brands fa-linkedin"></i>
            <p>Linkedin</p>
          </li>
        </a>
      </div>
    </div>
  </section>
</footer>
```

## Explicación de la Estructura

- **`<footer>`**: Elemento principal que define la sección del pie de página.

- **`<section class="section-footer">`**: Contenedor que envuelve toda la sección del pie de página.

- **`<h2 class="title-contact" id="contacto">`**: Título de la sección de contacto, con un estilo destacado y margen para el scroll.

- **`<div class="container-redes">`**: Contenedor que agrupa los enlaces a las redes sociales.

- **Enlaces `<a>`**: Enlaces a diferentes plataformas como **Whatsapp**, **Github**, **LinkedIn**:
  - **Whatsapp**: Enlace para enviar un mensaje a través de WhatsApp.
  - **Github**: Enlace al perfil de GitHub.
  - **LinkedIn**: Enlace al perfil de LinkedIn.

- **`<li class="li-contact">`**: Elementos de lista que contienen los iconos y texto descriptivo de cada red social.

## # Guía Código del Header `src/components/header`

## Descripción General

Este código proporciona un encabezado responsive para un portafolio. En dispositivos móviles, el menú de navegación se convierte en un menú desplegable que se activa y desactiva al hacer clic en el botón de menú. También se incluyen animaciones y transiciones para mejorar la experiencia del usuario.

### Estructura del HTML

1. **`<header class="header">`**: Este es el contenedor principal del encabezado, que incluye el título del portafolio y el menú de navegación.

2. **`<h1 id="inicio">Portafolio</h1>`**: Título principal del encabezado que define el nombre del portafolio. Este elemento está marcado con el ID "inicio", lo que puede ayudar para enlaces de navegación dentro de la página.

3. **`<nav class="nav">`**: Contenedor de navegación que agrupa los enlaces del menú.

4. **`<ul class="ul-nav">`**: Lista no ordenada que contiene los enlaces de navegación.

5. **Enlaces `<a>`**: Cada enlace tiene un `href` que apunta a una sección específica de la página:
    - **Inicio**: Enlace a la sección con ID `inicio`.
    - **Proyectos**: Enlace a la sección con ID `proyectos`.
    - **Habilidades**: Enlace a la sección con ID `skills`.
    - **Estudios**: Enlace a la sección con ID `estudios`.
    - **Sobre mí**: Enlace a la sección con ID `sobremi`.
    - **Contacto**: Enlace a la sección con ID `contacto`.

6. **`<div class="container-bnt-menu">`**: Contenedor que envuelve el botón de menú, visible solo en pantallas pequeñas.

7. **`<div class="btn-menu">`**: Botón que activa el menú desplegable en dispositivos móviles. Está compuesto de tres líneas representadas por los elementos `<span>`.

8. **`<div class="menu-drop"></div>`**: Un contenedor de fondo que aparece cuando el menú está activo. Proporciona un efecto de oscurecimiento en el fondo al abrir el menú.

### JavaScript

- Se utiliza para alternar clases y activar el menú de navegación móvil.
    - **`$btnmenu.addEventListener("click", () => {...})`**: Este bloque de código escucha un clic en el botón de menú y alterna las clases para mostrar/ocultar el menú y las animaciones de las líneas del botón.
    - **`$menuDrop.addEventListener("click", () => {...})`**: Este bloque de código asegura que al hacer clic fuera del menú (en el fondo), el menú se cierre y las líneas del botón de menú vuelvan a su estado original.

### Estilos CSS

1. **`header`**: Define el estilo general del encabezado:
    - `position: relative;` y `display: flex;`: Posiciona el encabezado de manera flexible y permite el alineamiento.
    - `background-color: #000;` y `color: #f6f6f9;`: Establece un fondo negro y un texto blanco para el encabezado.

2. **`nav`**: Estilo para la barra de navegación:
    - `display: flex;`: Utiliza flexbox para alinear los elementos de navegación de forma horizontal.
    - `justify-content: space-between;`: Espacia los elementos de forma equidistante.

3. **`ul-nav` y `li-nav`**: Define el estilo para los elementos de la lista de navegación:
    - `list-style: none;`: Elimina los puntos de la lista.
    - `transition: 0.3s;`: Añade una transición suave al pasar el mouse por encima de los elementos.

4. **Efectos de Hover**:
    - **`li-nav:hover::before`**: Muestra una línea verde debajo del texto cuando el usuario pasa el mouse sobre un elemento de navegación.
    - **`li-nav:hover`**: Cambia el color del texto al verde (#01be96) al pasar el mouse.

5. **Estilos para el botón de menú**:
    - **`linea-menu`**: Establece el estilo para las tres líneas que forman el icono del menú. Estas líneas tienen animaciones que las transforman al hacer clic.

### Estilos Responsivos

1. **`@media (max-width: 720px)`**: Los estilos dentro de esta consulta de medios se aplican cuando el ancho de la pantalla es de 720 píxeles o menos (dispositivos móviles).

    - **`menu-drop` y `container-bnt-menu`**: Ambos elementos se muestran solo en pantallas pequeñas. El contenedor del botón de menú (`container-bnt-menu`) se muestra y el menú desplegable (`menu-drop`) se activa.
    - **Animaciones para las líneas del menú**: Las líneas del botón de menú se transforman para crear una animación tipo "X" cuando se hace clic en ellas.
    - **`nav`**: El menú de navegación se convierte en una columna fija en la pantalla con un fondo oscuro cuando está activado.

2. **Interacción del menú**:
    - **`menu-activado`**: Aparece el menú en la pantalla a través de una transición desde la derecha, ocupando toda la altura de la pantalla.

3. **Fondo de menú**: Al hacer clic en el fondo oscuro (`menu-drop`), el menú se cierra.


# Guía de la Sección `src/const/const`

La sección `src/const/const` contiene varias constantes y configuraciones clave utilizadas en todo el proyecto. Estas constantes incluyen información sobre los estudios, habilidades, iconos y proyectos que forman parte del sistema, lo cual permite una mejor organización y reutilización del código.

## Contenido de `const.js`

El archivo `const.js` define tres estructuras principales:

1. **`studies`**: Una lista de estudios que contiene los títulos académicos y las fechas de los cursos.
2. **`IconKeys`**: Un objeto que asocia claves con íconos utilizados en la interfaz de usuario.
3. **`skills`**: Una lista de habilidades, cada una con un título y un ícono relacionado.
4. **`projects`**: Una lista de proyectos con detalles como imágenes, enlaces y tecnologías utilizadas.

### `studies` - Lista de Estudios

El array `studies` contiene una serie de objetos, cada uno representando un estudio o formación académica. Cada objeto tiene los siguientes atributos:

- **`title`**: El nombre del estudio o especialización.
- **`corporation`**: La institución que impartió el estudio.
- **`date`**: El período en que se cursó el estudio.

#### Ejemplo de Datos

```javascript
export const studies = [
  {
    title: "Estudiante de Ingeniería de Sistemas e Informática",
    corporation: "Universidad Continental Cusco",
    date: "2022-Actualidad",
  },
  // Otros estudios...
];
```

## Espero que la documentación sea de ayuda para modificar el proyecto "Portafolio" para que sea personalizado.
