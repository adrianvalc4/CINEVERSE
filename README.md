# CINEVERSE — Sitio de películas

Proyecto académico de Programación Web. Esta carpeta contiene la **primera entrega de estructura y estilos globales**; no incluye JavaScript ni funciones interactivas.

## Diseño en Figma

[ Abrir CINEVERSE en Figma ](https://www.figma.com/design/qIuaAyW3CqxVHsRy82nkDJ)

El archivo de Figma contiene la biblioteca de componentes y las pantallas iniciales de Inicio y Catálogo. En el plan Starter se organizó en tres páginas: `Componentes`, `Inicio + Catálogo` y `Detalle + Contacto`.

## Identidad visual

| Uso | Valor |
|---|---|
| Fondo principal | `#0F0F14` |
| Superficie / tarjetas | `#1C1C26` |
| Superficie elevada | `#252530` |
| Color principal | `#E50914` |
| Texto principal | `#FFFFFF` |
| Texto secundario | `#A0A0B0` |
| Bordes | `#383844` |
| Calificación | `#F4C46B` |
| Tipografía | Poppins |
| Radio principal | `8px` |
| Escala de espacios | múltiplos de `8px` |

Los colores, tamaños y espacios se centralizan en `css/styles.css`, dentro de `:root`. Para cambiar un color global, modifica su variable y no cada selector por separado.

## Estructura

```text
CINEVERSE/
├── index.html
├── catalogo.html
├── detalle.html
├── contacto.html
├── css/
│   └── styles.css
├── img/
└── docs/
```

## Header

El encabezado se repite en las páginas y contiene:

- `header.site-header`: contenedor semántico de la cabecera.
- `a.brand`: logotipo CINEVERSE y enlace a Inicio.
- `nav.primary-nav`: navegación principal.
- `a.nav-link`: enlaces Inicio, Catálogo y Contacto.
- `span.menu-toggle`: icono visual de menú móvil; todavía no tiene comportamiento.

La distribución se realiza con Flexbox: `display: flex`, `align-items: center` y `justify-content: space-between`.

## Qué incluye esta primera entrega

- Estructura semántica inicial de las cuatro páginas.
- Header común en HTML.
- Variables globales y reset CSS.
- Paleta de colores y tipografía Poppins.
- Primer uso de Flexbox en header, hero, tarjetas y footer.
- Ajuste visual para tablet y móvil.

## Qué queda para etapas posteriores

- Completar el contenido de Catálogo, Detalle y Contacto.
- Implementar el menú hamburguesa, filtros, buscador y validación del formulario.
- Añadir JavaScript y conexión con datos cuando lo indique el docente.
- Revisar y conectar las pantallas del prototipo de Figma.

## Cómo visualizar el proyecto

1. Abre esta carpeta en Visual Studio Code.
2. Abre `index.html` en el navegador, o usa la extensión Live Server.
3. Para revisar las otras estructuras, abre `catalogo.html`, `detalle.html` y `contacto.html`.

También se puede iniciar un servidor local desde una terminal ubicada en esta carpeta:

```bash
python -m http.server 5500
```

Después abre `http://localhost:5500` en el navegador.

## Git y GitHub

Este paquete se preparó para inicializar un repositorio local. Para publicarlo en GitHub, crea un repositorio vacío llamado `CINEVERSE` y conecta su URL remota. Las instrucciones están en `docs/GITHUB_PASO_A_PASO.md`.
