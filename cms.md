# Sistema de Gestión de Contenidos (CMS)

Un **CMS** (*Content Management System*) es una plataforma de software que permite crear, administrar, editar y publicar contenido digital en un sitio web sin necesidad de escribir código directamente ni gestionar bases de datos manualmente.

## ¿Para qué sirve?

Sirve para simplificar la creación y el mantenimiento de páginas web (como tiendas online, periódicos digitales, blogs o webs corporativas), permitiendo que usuarios sin conocimientos técnicos puedan actualizar el contenido de forma autónoma.

## Funcionamiento

Un CMS separa el contenido (guardado en una base de datos) de la presentación (plantillas visuales). El ciclo completo es este:

1. **Edición:** el creador de contenido escribe o modifica una página desde el panel de administración, y el CMS guarda el texto, las imágenes y los datos en la base de datos.
2. **Petición:** un visitante abre la página en su navegador y el servidor recibe la petición.
3. **Consulta:** el CMS, ejecutándose en el servidor (por ejemplo, en PHP), consulta a la base de datos el contenido que necesita.
4. **Plantilla:** el CMS inserta esos datos en la plantilla visual (cabecera, menús, diseño) y genera el HTML en ese momento.
5. **Respuesta:** el servidor envía el HTML al navegador, que lo muestra al visitante.

Este proceso se repite en cada visita, por eso un cambio guardado en el panel se ve de inmediato al recargar la página.

## ¿Cómo se clasifican?

Los CMS se pueden clasificar principalmente bajo dos criterios: su propósito y su arquitectura técnica.

### Según su propósito

- **CMS de uso general / blogs:** diseñados para publicaciones periódicas y webs informativas.
  - Ejemplos: WordPress, Joomla.
- **CMS de comercio electrónico (e-commerce):** especializados en catálogos de productos, carritos de compra y pasarelas de pago.
  - Ejemplos: Shopify, PrestaShop, Magento (Adobe Commerce).
- **CMS de documentación y aprendizaje (LMS):** orientados a estructurar cursos, guías o manuales.
  - Ejemplos: Moodle, Canvas.

### Según su arquitectura

- **CMS tradicional o monolítico:** la interfaz del usuario (frontend) y la gestión de la base de datos (backend) están completamente acopladas en el mismo sistema.
  - Ejemplos: WordPress, Drupal.
- **CMS en la nube / propietario (SaaS o *website builders*):** plataformas todo en uno donde el alojamiento, el diseño y la infraestructura los gestiona completamente el proveedor.
  - Ejemplos: Wix, Squarespace, Webflow.
- **CMS desacoplado o *headless* (sin cabeza):** separan por completo la gestión del contenido (backend) de la capa de visualización (frontend). El contenido se entrega únicamente a través de APIs (REST/GraphQL) a cualquier dispositivo (web, app móvil, pantalla inteligente).
  - Ejemplos: Contentful, Strapi, Sanity, Ghost (usado como headless).

## Top 5 de CMS más usados

Ranking según W3Techs, con datos del **26 de octubre de 2026**. Se muestran dos medidas distintas, porque cambian mucho el resultado:

- **Uso sobre todas las webs:** porcentaje del total de sitios web analizados.
- **Cuota de mercado:** porcentaje solo entre las webs cuyo CMS es conocido.

| Posición | CMS | Uso sobre todas las webs | Cuota de mercado (webs con CMS conocido) |
| :---: | :--- | :---: | :---: |
| 1 | WordPress | 39,6 % | 58,3 % |
| 2 | Shopify | 5,3 % | 7,9 % |
| 3 | Wix | 4,2 % | 6,2 % |
| 4 | Squarespace | 2,4 % | 3,6 % |
| 5 | Joomla | 1,1 % | 1,6 % |

Además, el 32,1 % de las webs analizadas no usa ninguno de los CMS que W3Techs monitoriza.

**Fuente:** [W3Techs, Usage statistics and market shares of content management systems](https://w3techs.com/technologies/overview/content_management), consultado el 26 de octubre de 2026.

## Comparativa: CMS dinámico frente a generador estático (SSG)

| Aspecto | CMS dinámico | Generador estático (SSG) |
| :--- | :--- | :--- |
| **Forma de crear contenidos** | A través de un panel de administración visual (*dashboard*) con editores WYSIWYG o bloques. | Redactando archivos de texto plano (principalmente en formato Markdown) en un editor de código. |
| **Base de datos** | Sí (utiliza bases de datos relacionales como MySQL o PostgreSQL para consultar el contenido). | No (el contenido reside directamente en el sistema de archivos del proyecto). |
| **Generación del HTML** | En tiempo real / bajo demanda (se compila dinámicamente cada vez que un usuario solicita la página). | Por adelantado (se compila durante la fase de *build*, previo a la publicación). |
| **Servidor necesario** | Servidor de aplicaciones activo que ejecute un lenguaje backend (PHP, Node.js, Python, etc.) y la base de datos. | Servidor web simple o CDN (*Content Delivery Network*) para entregar archivos estáticos. |
| **Panel de administración** | Sí, integrado de forma nativa para gestionar la web visualmente sin tocar código. | No por defecto (opcionalmente se puede integrar un Headless CMS o un CMS basado en Git). |
| **Conocimientos técnicos** | Bajos para el creador de contenido; medio-altos solo para el mantenimiento o el desarrollo inicial. | Medios a altos (requiere uso de la consola/terminal, Git y sintaxis de motores de plantillas). |
| **Seguridad** | Menor (al estar expuesto a bases de datos y backend, es más susceptible a inyecciones SQL, vulnerabilidades en plugins y ataques de fuerza bruta). | Alta (al no tener base de datos ni procesamiento en servidor en tiempo real, la superficie de ataque es mínima). |
| **Rendimiento** | Variable / menor (requiere procesamiento en servidor y consultas a la BD, aunque se mitigue con sistemas de caché). | Máximo (la carga es casi instantánea al servir archivos HTML directos desde una CDN). |
| **Actualización del contenido** | Inmediata; los cambios guardados en el panel se reflejan al recargar la página. | Requiere recompilación (*rebuild*): hay que regenerar el proyecto y subir los archivos actualizados al servidor. |
| **Publicación** | Se guarda el cambio en el panel y la base de datos lo sirve en tiempo real. | Se hace un *build* del proyecto y se despliega la carpeta de salida a un servicio de hosting o CDN (vía Git/CI-CD). |
| **Ejemplos** | WordPress, Joomla, Drupal, PrestaShop. | Jekyll, Hugo, Astro, Eleventy, Gatsby. |

## Recursos adicionales

- [Vídeo explicativo sobre CMS](https://www.youtube.com/watch?v=OBJP4dvoS_I) (duración: 3:22 min)
- [Ver documento sobre Generadores de Sitios Estáticos (ssg.md)](ssg.md)
