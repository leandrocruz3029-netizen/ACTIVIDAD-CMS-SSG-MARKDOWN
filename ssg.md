# ¿Qué es un SSG?
--> Es una herramienta que genera un sitio web HTML estático completo a partir de datos brutos y un conjunto de plantillas.

## Comparativa de Herramientas Líderes: Jekyll, Hugo y Astro

| Aspecto | Jekyll | Hugo | Astro |
| :--- | :--- | :--- | :--- |
| **Tecnología o lenguaje principal** | Ruby | Go / Golang | JavaScript / TypeScript |
| **Formato utilizado para el contenido** | Markdown | Markdown, Org-mode | Markdown, MDX y componentes .astro |
| **Necesidad de instalación** | Ruby, RubyGems, GCC y Make | Un único archivo binario sin dependencias externas | Node.js y gestor de paquetes (npm/pnpm) |
| **Funcionamiento básico** | Compila contenido en Markdown combinándolo con plantillas Liquid | Compila plantillas y Markdown en paralelo mediante un ejecutable | Genera HTML estático e inyecta JS interactivo solo donde se necesita (arquitectura de islas) |
| **Usos habituales** | Blogs sencillos, webs personales y documentación en GitHub Pages | Webs masivas con gran volumen de páginas, blogs y documentación extensa | Portafolios modernos, aplicaciones web híbridas y sitios que combinan varios frameworks |
| **Ventajas** | Integración nativa sin configuración previa en GitHub Pages; muy maduro y con gran comunidad | Velocidad de compilación extrema; instalación en un solo binario sin dependencias complejas | Permite componentes de React, Vue o Svelte; rendimiento superior enviando cero JS al cliente por defecto |
| **Inconvenientes** | Tiempos de compilación lentos en proyectos grandes; gestión molesta de dependencias en Ruby | Curva de aprendizaje empinada para la sintaxis de sus plantillas y estructura de carpetas | Relativamente más reciente; mayor sobrecarga si solo se busca hacer un blog en texto plano sencillo |
| **Publicación en GitHub Pages** | Sí (Nativo directamente sin configurar acciones CI/CD complejas) | Sí (Mediante ejecutable directo o automatizado con GitHub Actions) | Sí (A través de GitHub Actions para compilar la carpeta de salida) |

## Video explicativo sobre SSG
[SSG](https://www.youtube.com/watch?v=osWfEtbP_sk&pp=ygUydmlkZW8gZXhwbGljYXRpdm8gc29icmUgc3NnIFN0YXRpYyBTaXRlIEdlbmVyYXRvcik%3D)

### enlace a la siguiente página CMS
**[Ver documento sobre Content Managment System (cms.md)](cms.md)**