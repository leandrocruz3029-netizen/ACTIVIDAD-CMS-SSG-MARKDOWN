# ¿Qué es un SSG?
--> Es una herramienta que genera un sitio web HTML estático completo a partir de datos brutos y un conjunto de plantillas.

## Comparativa de Herramientas Líderes: Jekyll, Hugo y Astro

| Aspecto | Jekyll | Hugo | Astro |
| :--- | :--- | :--- | :--- |
| **Tecnología o lenguaje principal** | Ruby[cite: 5, 7] | Go / Golang[cite: 5, 7] | JavaScript / TypeScript[cite: 5, 7] |
| **Formato utilizado para el contenido** | Markdown[cite: 7] | Markdown, Org-mode[cite: 7] | Markdown, MDX y componentes .astro[cite: 7] |
| **Necesidad de instalación** | Ruby, RubyGems, GCC y Make[cite: 7] | Un único archivo binario sin dependencias externas[cite: 7, 8] | Node.js y gestor de paquetes (npm/pnpm)[cite: 7] |
| **Funcionamiento básico** | Compila contenido en Markdown combinándolo con plantillas Liquid[cite: 7] | Compila plantillas y Markdown en paralelo mediante un ejecutable[cite: 7, 8] | Genera HTML estático e inyecta JS interactivo solo donde se necesita (arquitectura de islas)[cite: 7] |
| **Usos habituales** | Blogs sencillos, webs personales y documentación en GitHub Pages[cite: 5, 8] | Webs masivas con gran volumen de páginas, blogs y documentación extensa[cite: 5, 8] | Portafolios modernos, aplicaciones web híbridas y sitios que combinan varios frameworks[cite: 5, 8] |
| **Ventajas** | Integración nativa sin configuración previa en GitHub Pages; muy maduro y con gran comunidad[cite: 5, 8] | Velocidad de compilación extrema; instalación en un solo binario sin dependencias complejas[cite: 5, 8] | Permite componentes de React, Vue o Svelte; rendimiento superior enviando cero JS al cliente por defecto[cite: 5, 8] |
| **Inconvenientes** | Tiempos de compilación lentos en proyectos grandes; gestión molesta de dependencias en Ruby[cite: 8] | Curva de aprendizaje empinada para la sintaxis de sus plantillas y estructura de carpetas[cite: 8] | Relativamente más reciente; mayor sobrecarga si solo se busca hacer un blog en texto plano sencillo[cite: 8] |
| **Publicación en GitHub Pages** | Sí (Nativo directamente sin configurar acciones CI/CD complejas)[cite: 8] | Sí (Mediante ejecutable directo o automatizado con GitHub Actions)[cite: 8] | Sí (A través de GitHub Actions para compilar la carpeta de salida)[cite: 8] |

## Video explicativo sobre SSG
[SSG](https://www.youtube.com/watch?v=osWfEtbP_sk&pp=ygUydmlkZW8gZXhwbGljYXRpdm8gc29icmUgc3NnIFN0YXRpYyBTaXRlIEdlbmVyYXRvcik%3D)

### enlace a la siguiente página CMS
**[Ver documento sobre Content Managment System (cms.md)](cms.md)**