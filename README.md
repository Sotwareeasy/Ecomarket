#  EcoMarket

Tienda en línea de productos ecológicos, reutilizables y sustentables, maquetada con **HTML5 semántico y CSS3 puro** (cero JavaScript, cero frameworks), siguiendo la metodología **BEM** para nombrar clases.

> Proyecto académico — Módulo HTML + CSS.

## 📖 Descripción del proyecto

EcoMarket ofrece una plataforma accesible y atractiva donde los usuarios pueden explorar productos ecológicos, conocer sus beneficios y "realizar" compras responsables. El proyecto consta de 4 vistas:

| Vista | Archivo | Descripción |
|---|---|---|
| Inicio | `index.html` | Hero, productos destacados y franja de principios. |
| Productos | `views/productos.html` | Catálogo de 20 productos con sidebar de filtros (sticky), buscador y paginación visual. |
| Sobre Nosotros | `views/sobre-nosotros.html` | Historia de la marca, principios ecológicos y carrusel de testimonios (100% CSS con `scroll-snap`). |
| Contacto | `views/contacto.html` | Formulario con validación visual `:valid` / `:invalid`, mapa estático y redes sociales. |

Toda la interactividad (menú móvil, favoritos, validación de formulario) se resuelve con **selectores avanzados de CSS** (`:checked`, `:valid`, `:invalid`, `:active`, `:target`, `:focus-visible`), sin una sola línea de JavaScript.

## 🚀 Instrucciones de visualización

### Opción 1 — Ver en línea (recomendado)
Abre el sitio ya desplegado: ** **

### Opción 2 — Ejecutar localmente
1. Clona el repositorio:
   ```bash
   git clone https://github.com/Sotwareeasy/Ecomarket.git
   ```
2. Abre `index.html` directamente en tu navegador, **o** sirve la carpeta con un servidor estático simple:
   ```bash
   npx serve .
   # o
   python3 -m http.server 5500
   ```
3. Navega a `http://localhost:5500`.



## 🛠️ Tecnologías utilizadas

- **HTML5 semántico** (`header`, `nav`, `main`, `section`, `article`, `aside`, `footer`).
- **CSS3 puro**: Custom Properties (variables), Flexbox, Grid, `scroll-snap`, pseudo-clases (`:hover`, `:active`, `:target`, `:checked`, `:valid`, `:invalid`, `:focus-visible`), `@keyframes`.
- **Metodología BEM** (`bloque__elemento--modificador`) para la nomenclatura de clases.
- **SVG** para ilustraciones e iconografía (sin dependencias externas de imágenes).
- **Mobile First**: todos los estilos parten de la vista móvil y escalan con `min-width`.
- **Despliegue**: Vercel / Netlify (sitio 100% estático).

## 📁 Estructura de archivos

```
EcoMarket/
├── css/
│   ├── main.css            # Reset, variables (design tokens), tipografía base
│   ├── layout.css          # Header, Footer, grid systems, sidebar
│   ├── components.css      # Cards, botones, inputs, filtros, paginación, carrusel
│   └── animations.css      # Keyframes y transiciones
├── img/
│   ├── products/            # Ilustraciones SVG de productos
│   ├── icons/                # Iconos de principios, avatares y mapa
│   └── hero/                 # Ilustración del banner principal
├── views/
│   ├── productos.html
│   ├── sobre-nosotros.html
│   └── contacto.html
├── index.html               # Home
└── README.md
```

## 🎨 Sistema de diseño

| Token | Valor | Uso |
|---|---|---|
| `--color-forest-900` | `#143726` | Texto de marca, footer |
| `--color-green-700` | `#27ae60` | Botones primarios, acentos |
| `--color-green-500` | `#2ecc71` | Detalles, logotipo |
| `--color-sand-100` | `#f5f5dc` | Fondos secundarios |
| `--color-clay-500` | `#e6c068` | Estrellas, acentos cálidos |

Tipografía: fuente serif del sistema (`Georgia`) para títulos y fuente sans-serif del sistema (`system-ui`) para texto, priorizando legibilidad y tiempo de carga cero (sin fuentes externas).

## 📱 Responsividad

Enfoque **Mobile First** con puntos de quiebre en `620px`, `900px` y `1000px`:

- **Catálogo**: 1 columna (móvil) → 2 columnas (tablet, `≥620px`) → 4 columnas (escritorio, `≥1000px`).
- **Menú**: panel deslizable a pantalla completa en móvil (checkbox hack, sin JS) → barra horizontal en escritorio (`≥900px`).
- **Historia (Sobre Nosotros)**: columna apilada en móvil → fila con Flexbox en pantallas ≥800px.

## 📸 Capturas de pantalla

> Agrega aquí las capturas de escritorio y móvil de cada vista tras el despliegue.

| Vista | Escritorio | Móvil |
|---|---|---|
| Inicio | _(agregar imagen)_ | _(agregar imagen)_ |
| Productos | _(agregar imagen)_ | _(agregar imagen)_ |
| Sobre Nosotros | _(agregar imagen)_ | _(agregar imagen)_ |
| Contacto | _(agregar imagen)_ | _(agregar imagen)_ |

## 🌿 Autor
Fabian Uribe