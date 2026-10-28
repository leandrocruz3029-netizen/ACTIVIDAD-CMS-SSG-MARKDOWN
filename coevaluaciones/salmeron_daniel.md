# COEVALUACIÓN DE CMS Y SSG

**Nombre del evaluador:** [Daniel Salmerón Gallardo].
**Persona evaluada:** [Leandro Cruz].
**Mi repositorio:** [https://github.com/dgal-89/gestoresContenido.git].
**Repositorio que evalúo:** [https://github.com/leandrocruz3029-netizen/ACTIVIDAD-CMS-SSG-MARKDOWN.git].

## A. Puntuación de la investigación

| Código | Criterio | Máximo | Puntos asignados | Evidencia y justificación concreta |
| :--- | :--- | :---: | :---: | :--- |
| A1 | Concepto y funcionamiento de SSG. | 1 | 0,5 | ssg.md, apartado "¿Qué es un SSG?": la definición es correcta, pero ocupa una sola línea y no explica el funcionamiento (contenido en Markdown + plantillas + configuración → build → carpeta de salida con HTML → publicación). |
| A2 | SSG frente a HTML manual. | 0,5 | 0,5 | No aparece en ssg.md ningún apartado que compare un SSG con escribir el HTML a mano. |
| A3 | Comparación de Jekyll, Hugo y Astro. | 1 | 1 | ssg.md, tabla comparativa: incluye los 8 aspectos (tecnología, formato, instalación, funcionamiento, usos, ventajas, inconvenientes y GitHub Pages) con datos concretos y correctos. |
| A4 | Concepto y funcionamiento de CMS. | 1 | 1 | cms.md, apartados iniciales: la definición es correcta, pero el apartado "Funcionamiento" explica para qué sirve un CMS y no cómo funciona (panel de administración, base de datos, plantillas y generación de la página en cada petición). |
| A5 | Clasificación de CMS y ejemplos. | 0,5 | 0,5 | cms.md, "¿Cómo se clasifican?": separa por propósito (general, e-commerce, LMS) y por arquitectura (monolítico, SaaS, headless), con ejemplos en cada tipo. |
| A6 | Top 5 y estadísticas de mercado. | 0,5 | 0 | No hay ranking, fuente, fecha de los datos ni medida usada en ninguno de los dos documentos. |
| A7 | Comparativa CMS dinámico–SSG. | 1 | 1 | cms.md, tabla comparativa: 11 aspectos completos (contenido, base de datos, generación del HTML, servidor, panel, conocimientos, seguridad, rendimiento, actualización, publicación y ejemplos). |
| A8 | Claridad y apoyo visual. | 0,5 | 0,50 | Las dos tablas se leen bien, pero no hay ninguna imagen ni esquema, y la clasificación de CMS es texto plano sin subtítulos ni listas, lo que dificulta seguirla. |
| **Subtotal A** | | **6** | **5,75** | |

## B. Puntuación de la actividad Markdown

| Código | Criterio | Máximo | Puntos asignados | Evidencia y justificación concreta |
| :--- | :--- | :---: | :---: | :--- |
| B1 | Organización del proyecto. | 0,75 | 0,5 | Existen cms.md y ssg.md con nombres correctos. No hay carpeta de recursos porque no se usan imágenes. [Comprobar estructura en el repositorio]. |
| B2 | Adaptación de la investigación. | 0,75 | 0,5 | La mayor parte de la investigación está adaptada a Markdown, pero faltan secciones: funcionamiento de SSG y SSG frente a HTML manual en ssg.md, y Top 5 de CMS en cms.md. |
| B3 | Sintaxis Markdown. | 0,5 | 0,25 | Tablas, negritas y enlaces correctos. Problemas: se usa "-->" como texto, la clasificación no usa encabezados (###) ni listas (-), cms.md tiene tres títulos H1, y el enlace del vídeo de CMS está entre paréntesis "([CMS](...))", que se ven en la vista previa. |
| B4 | Imágenes y rutas. | 0,5 | 0,5 | Ninguno de los dos documentos incluye imágenes. |
| B5 | Dos vídeos de hasta 5 minutos. | 0,5 | 0,5 | Enlace CMS presente, duración: [mm:ss]. Enlace SSG presente, duración: [mm:ss]. El enlace de SSG arrastra un parámetro de búsqueda (&pp=...) que se podría eliminar.. |
| B6 | Enlace de cms.md a ssg.md. | 0,5 | 0,5 | Al final de cms.md hay un enlace relativo a ssg.md que abre correctamente. Además ssg.md enlaza de vuelta a cms.md. |
| B7 | Legibilidad de ambos documentos. | 0,5 | 0,25 | En la vista previa las tablas se leen bien, pero la clasificación de CMS aparece como bloque de párrafos sin jerarquía. Hay una errata: "Managment" en lugar de "Management" en ssg.md. |
| **Subtotal B** | | **4** | **3,5** | |

## C. Nota propuesta y valoración inicial

- **Puntuación real A + B:** 8 / 10.

**Justificación de la nota:**
Las dos tablas comparativas (Jekyll/Hugo/Astro y CMS dinámico frente a SSG) están completas y obtienen la puntuación máxima, y la clasificación de CMS es correcta. La nota baja porque faltan tres contenidos de la investigación (funcionamiento de SSG, SSG frente a HTML manual y Top 5 de CMS), no hay imágenes y el formato Markdown de la clasificación es mejorable. La nota es provisional hasta confirmar la duración de los vídeos y la estructura del repositorio.

**Dos puntos fuertes:**

- **Tabla CMS dinámico frente a SSG (cms.md):** cubre 11 aspectos con explicaciones concretas, por ejemplo por qué un SSG es más seguro (no hay base de datos ni procesamiento en el servidor). Permite entender de un vistazo cuándo conviene cada opción.
- **Tabla Jekyll, Hugo y Astro (ssg.md):** incluye detalles prácticos, como que Hugo es un único binario sin dependencias o que Astro usa arquitectura de islas. Ayuda a elegir herramienta según el proyecto y no solo a conocerlas.

**Dos mejoras prioritarias:**

| Propuesta | Archivo y apartado | Observación y mejora propuesta |
| :--- | :--- | :--- |
| P1 | cms.md: nuevo apartado "Top 5 de CMS" (antes de la comparativa). | Falta el ranking de CMS más usados. Añadir una tabla con los 5 primeros, indicando la fuente (por ejemplo W3Techs), la fecha de consulta y la medida usada (porcentaje del total de webs o cuota entre webs que usan CMS), porque son dos cifras distintas. |
| P2 | ssg.md: apartado "¿Qué es un SSG?". | La definición es de una sola línea. Añadir un apartado "¿Cómo funciona?" con el proceso (contenido Markdown + plantillas + configuración → build → carpeta de salida → hosting), idealmente con un esquema como imagen, y un apartado "SSG frente a HTML manual" con sus ventajas (plantillas reutilizables, cambios globales en un solo sitio, Markdown en lugar de HTML). |
| P3 (opcional) | cms.md: "Funcionamiento" y "¿Cómo se clasifican?". | "Funcionamiento" explica para qué sirve, no cómo funciona: explicar el ciclo petición → consulta a la base de datos → plantilla → HTML. En la clasificación, usar ### para "Según su propósito" y "Según su arquitectura", listas con guiones para cada tipo y sustituir "-->" por texto normal. |

## D. Respuesta y correcciones del propietario del proyecto

**Cumplimenta:** Leandro Cruz.

| Propuesta | Respuesta y decisión razonada | Corrección aplicada y archivo | Commit |
| :--- | :--- | :--- | :--- |
| P1 | Aceptada. Sin ranking, fuente ni fecha no se puede valorar la cuota real de cada CMS, y la medida usada cambia mucho el resultado (uso sobre todas las webs frente a cuota entre webs con CMS conocido). | En cms.md he añadido el apartado "Top 5 de CMS más usados", antes de la comparativa, con una tabla de ranking, la fuente (W3Techs), la fecha de consulta (26/10/2026) y las dos medidas por separado. | [Ver commit](https://github.com/leandrocruz3029-netizen/ACTIVIDAD-CMS-SSG-MARKDOWN/commit/b8b2d6c). |
| P2 | Aceptada. Una definición de una sola línea no explica cómo trabaja un SSG ni por qué compensa frente a escribir HTML a mano. | En ssg.md he añadido los apartados "¿Cómo funciona?" (contenido, plantillas, build, carpeta de salida y publicación) y "SSG frente a HTML manual", con una tabla comparativa. | [Ver commit](https://github.com/leandrocruz3029-netizen/ACTIVIDAD-CMS-SSG-MARKDOWN/commit/1c775a1). |
| P3 (opcional) | Aceptada. El apartado "Funcionamiento" explicaba para qué sirve un CMS, no cómo funciona, y la clasificación era un bloque de texto sin jerarquía. | En cms.md he reescrito "Funcionamiento" como un ciclo de 5 pasos y he estructurado la clasificación con `###` y listas, quitando los "-->". | [Ver commit](https://github.com/leandrocruz3029-netizen/ACTIVIDAD-CMS-SSG-MARKDOWN/commit/b8b2d6c). |

**Qué he aprendido al corregir mi trabajo:** Al corregir mi trabajo he visto que en `cms.md` y `ssg.md` explicaba bien qué es un CMS y un SSG, pero no cómo funcionan por dentro. Por eso he añadido el ciclo completo de un CMS (edición, petición, consulta a la base de datos, plantilla y respuesta) y el proceso de un SSG (contenido, plantillas, build, carpeta de salida y publicación). También he aprendido que una estadística sin fuente, fecha y medida no se puede comprobar. Al hacer el Top 5 de CMS descubrí que "uso sobre todas las webs" y "cuota entre webs con CMS conocido" son cifras distintas, y que mezclarlas lleva a conclusiones erróneas. Por último, estructurar el texto con títulos y listas, en lugar de párrafos sueltos, hace que el documento se entienda mucho mejor. Y trabajar con ramas y Pull Requests me ha enseñado a corregir sobre la misma rama, y a dejar cada cambio en un commit que se pueda enlazar.
