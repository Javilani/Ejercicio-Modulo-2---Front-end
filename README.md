
# Ejercicio 2 - Página Web Hospital Akilar con HTML, CSS, SASS y Media Query

Este es un proyecto de una página web para el hospital Akilar, diseñado con HTML y CSS. El sitio web presenta información básica del hospital, incluyendo una página de bienvenida, detalles sobre el equipo médico y una sección de contacto.

## Descripción del Proyecto

La página web del Hospital Akilar consta de tres secciones principales:

**1. Página de Bienvenida (index.html):** Página de bienvenida que incluye una introducción al hospital, un apartado sobre los servicios que ofrece y una sección de testimonios de pacientes, proporcionando confianza a los nuevos visitantes.

**2. Equipo Médico (equipoMedico.html):** Página que muestra el equipo médico con una foto de cada uno, una breve descripción de cada miembro y su especialidad.

**3. Contacto (contacto.html):** Página de contacto con un formulario para que los usuarios puedan enviar mensajes y un mapa interactivo que muestra la ubicación del hospital.

Cada página cuenta con un archivo CSS independiente para estilizar el contenido.

#### Tecnologías utilizadas
- HTML
- CSS
- SASS
- Media Query


# Proyecto de Estilos Responsivos con SASS

Este proyecto tiene como objetivo crear un diseño responsivo para una página web utilizando SASS para la modularización de los estilos. Se implementan media queries para asegurar que el diseño se adapte correctamente a diferentes tamaños de pantalla, desde dispositivos móviles hasta escritorios grandes.

## Modularización de los Estilos y Media Queries

Para mantener el código limpio y organizado, se implementó la **modularización de los estilos** usando SASS. Esto permitió dividir los estilos en archivos parciales reutilizables. Además, se utilizó **media queries** para adaptar el diseño a diferentes tamaños de pantalla (móviles, tabletas, laptops y escritorios grandes).

### Media Queries

Las media queries están basadas en los siguientes puntos de interrupción (breakpoints):

- **$breakpoint-small:** 576px
- **$breakpoint-medium:** 768px
- **$breakpoint-large:** 1024px

Se implementaron en diversas secciones del proyecto para hacer que los elementos del diseño se ajusten de manera fluida dependiendo del tamaño de la pantalla:

- Para pantallas pequeñas (menos de 576px), se usan modificaciones como cambiar la orientación de los elementos de fila a columna, reducir márgenes, etc.
- Para pantallas medianas (entre 576px y 768px), se ajustan algunos elementos para mejorar la usabilidad en tabletas.
- Para pantallas grandes (mayores de 768px), se aplica un diseño más amplio y espacioso.

### Estructura de los Archivos SASS

La estructura de los archivos SASS y del proyecto en general está organizada de la siguiente manera para promover la reutilización y facilitar el mantenimiento:


        /HospitalAkilar
        │
        ├── index.html                
        ├── equipoMedico.html         
        ├── contacto.html             
        │
        ├── assets/
        │   ├── css/
        │   │   ├── style.css
        │   │   ├── style.css.map
        │   │   ├── styleContacto.css 
        │   │   ├── styleContacto.css.map
        │   │   ├── styleEM.css  
        │   │   └── styleEM.css.map
        │   │
        │   ├── scss/
        │   │   ├── style.scss
        │   │   ├── styleContacto.scss 
        │   │   ├── styleEM.scss
        │   │   ├── abstract
        │   │   │   └── _variables.scss
        │   │   ├── base
        │   │   ├── components
        │   │   ├── layout
        │   │   │   ├── _footer.scss
        │   │   │   └── _header.scss
        │   │   ├── pages
        │   │   │   ├── _contacto.scss
        │   │   │   ├── _equipoMedico.scss
        │   │   │   └── _index.scss
        │   │   ├── themes
        │   │   │   └── _default.scss
        │   │   └── vendors
        │   │
        │   └── img/                  
        │       ├── consultas.jpg
        │       ├── doctor-antonio.webp
        │       ├── doctor-carlos.jpeg
        │       ├── doctora-isabel.avif  
        │       ├── doctora-laura.avif      
        │       ├── especialidades.png   
        │       ├── facebook.png    
        │       ├── hospital.jpg  
        │       ├── instagram.png 
        │       ├── Logo-hospital.jpg    
        │       └── urgencias.png            
        │
        ├── node_modules
        ├── .gitignore
        ├── package-lock.json
        ├── package.json
        └── README.md                 

## Instrucciones para Visualizar el Proyecto

### Requisitos Previos

- Tener **Node.js** y **npm** instalados en tu computadora.
- Tener **SASS** instalado globalmente. Si no lo tienes, puedes instalarlo ejecutando el siguiente comando:

        npm install -g sass

### Pasos para Ejecutar el Proyecto

1. Clona el repositorio en tu máquina local:

        git clone <URL del repositorio>
        cd <nombre del repositorio>
2. Instala las dependencias necesarias (si es que usas alguna para el proyecto):

        npm install
3. Compila los archivos SASS en CSS ejecutando el siguiente comando:

        sass --watch assets/scss:assets/css
4. Abre el archivo index.html (o cualquier otro archivo HTML del proyecto) en tu navegador:
- Utiliza Live Server (si estás trabajando en VS Code) para ver la página en tu navegador
- Haz clic derecho sobre index.html.
- Selecciona "Open with Live Server" para iniciar la página en tu navegador.

## Authors

- [Javier Lagos](https://www.linkedin.com/in/javier-lagos-nieto-557169220/)

