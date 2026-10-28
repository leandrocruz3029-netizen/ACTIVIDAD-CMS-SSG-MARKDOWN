# Generadores de Sitios Estáticos (SSG)

## ¿Qué es un SSG?

Un **SSG** (*Static Site Generator*) es una herramienta que genera un sitio web HTML estático completo a partir de datos brutos (normalmente archivos de texto en Markdown) y un conjunto de plantillas.

## ¿Cómo funciona?

El trabajo del SSG ocurre **antes de publicar**, no cuando entra un visitante:

1. **Contenido:** se escribe en archivos de texto plano, normalmente Markdown (`.md`).
2. **Plantillas y configuración:** se definen las plantillas (cabecera, menú, diseño de página) y un archivo de configuración con los datos generales del sitio.
3. **Build:** el SSG combina el contenido con las plantillas y genera una página HTML por cada archivo.
4. **Carpeta de salida:** el resultado es una carpeta con HTML, CSS, JavaScript e imágenes ya terminados, sin base de datos ni código de servidor.
5. **Publicación:** esa carpeta se sube a un hosting estático o CDN (por ejemplo, GitHub Pages), y el servidor solo entrega archivos ya preparados.

Cuando se cambia un contenido, hay que repetir el *build* y volver a publicar.

## SSG frente a HTML manual

| Aspecto | HTML manual | SSG |
| :--- | :--- | :--- |
| **Contenido** | Se escribe con etiquetas HTML en cada página. | Se escribe en Markdown, más sencillo y legible. |
| **Elementos repetidos** (cabecera, menú, pie) | Se copian en todas las páginas. | Se definen una vez en una plantilla y se reutilizan. |
| **Cambios globales** | Hay que editar página por página, con riesgo de olvidar alguna. | Se cambia la plantilla y se regeneran todas las páginas a la vez. |
| **Sitios con muchas páginas** | Muy laborioso y propenso a errores. | Escala bien: un solo contenido genera cientos de páginas. |
| **Herramientas** | Solo un editor de texto. | Requiere instalar el generador y ejecutar el *build*. |
| **Resultado final** | HTML estático. | HTML estático (igual de rápido y seguro). |

En resumen, el SSG conserva las ventajas del HTML estático (rapidez, seguridad y hosting barato) y evita el trabajo repetitivo de escribir cada página a mano.

## Comparativa de herramientas líderes: Jekyll, Hugo y Astro

| Aspecto | Jekyll | Hugo | Astro |
| :--- | :--- | :--- | :--- |
| **Tecnología o lenguaje principal** | Ruby | Go / Golang | JavaScript / TypeScript |
| **Formato utilizado para el contenido** | Markdown | Markdown, Org-mode | Markdown, MDX y componentes .astro |
| **Necesidad de instalación** | Ruby, RubyGems, GCC y Make | Un único archivo binario sin dependencias externas | Node.js y gestor de paquetes (npm/pnpm) |
| **Funcionamiento básico** | Compila contenido en Markdown combinándolo con plantillas Liquid | Compila plantillas y Markdown en paralelo mediante un ejecutable | Genera HTML estático e inyecta JS interactivo solo donde se necesita (arquitectura de islas) |
| **Usos habituales** | Blogs sencillos, webs personales y documentación en GitHub Pages | Webs masivas con gran volumen de páginas, blogs y documentación extensa | Portafolios modernos, aplicaciones web híbridas y sitios que combinan varios frameworks |
| **Ventajas** | Integración nativa sin configuración previa en GitHub Pages; muy maduro y con gran comunidad | Velocidad de compilación extrema; instalación en un solo binario sin dependencias complejas | Permite componentes de React, Vue o Svelte; rendimiento superior enviando cero JS al cliente por defecto |
| **Inconvenientes** | Tiempos de compilación lentos en proyectos grandes; gestión molesta de dependencias en Ruby | Curva de aprendizaje empinada para la sintaxis de sus plantillas y estructura de carpetas | Relativamente más reciente; mayor sobrecarga si solo se busca hacer un blog en texto plano sencillo |
| **Publicación en GitHub Pages** | Sí (nativo, directamente sin configurar acciones CI/CD complejas) | Sí (mediante ejecutable directo o automatizado con GitHub Actions) | Sí (a través de GitHub Actions para compilar la carpeta de salida) |

## Vídeo explicativo sobre SSG

[Vídeo explicativo sobre SSG](https://www.youtube.com/watch?v=osWfEtbP_sk) (duración: 4:26 min)

## Enlace a la siguiente página

[Ver documento sobre Content Management System (cms.md)](cms.md)
