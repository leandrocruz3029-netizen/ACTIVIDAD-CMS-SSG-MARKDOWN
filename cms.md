# Sistema de Gestión de Contenidos (CMS)
--> Un CMS (Content Management System) es una plataforma de software que permite crear, administrar, editar y publicar contenido digital en un sitio web sin necesidad de escribir código directamente ni gestionar bases de datos manualmente.

# Funcionamiento 
--> Sirve para simplificar la creación y el mantenimiento de páginas web (como tiendas online, periódicos digitales, blogs o webs corporativas), permitiendo que usuarios sin conocimientos técnicos puedan actualizar el contenido de forma autónoma.

# ¿Cómo se clasifican?
--> Los CMS se pueden clasificar principalmente bajo dos criterios: su propósito y su arquitectura técnica.

Según su propósito

CMS de uso general / Blogs: Diseñados para publicaciones periódicas y webs informativas.

Ejemplos: WordPress, Joomla.

CMS de Comercio Electrónico (E-commerce): Especializados en catálogos de productos, carritos de compra y pasarelas de pago.

Ejemplos: Shopify, PrestaShop, Magento (Adobe Commerce).

CMS de Documentación y Aprendizaje (LMS): Orientados a estructurar cursos, guías o manuales.

Ejemplos: Moodle, Canvas.

Según su arquitectura

CMS Tradicional o Monolítico: La interfaz del usuario (frontend) y la gestión de 
la base de datos (backend) están completamente acopladas en el mismo sistema.

Ejemplos: WordPress, Drupal.

CMS Acoplado en la nube / Propietario (SaaS / Website Builders):
Plataformas todo en uno donde el alojamiento, el diseño y la infraestructura son gestionados completamente por el proveedor.

Ejemplos: Wix, Squarespace, Webflow.

CMS Desacoplado o Headless (Sin cabeza): Separan por completo la gestión 
del contenido (backend) de la capa de visualización (frontend). El contenido se entrega únicamente a 
través de APIs (REST/GraphQL) a cualquier dispositivo (web, app móvil, pantalla inteligente).

Ejemplos: Contentful, Strapi, Sanity, Ghost (usado como headless).


## Comparativa: CMS Dinámico frente a Generador Estático (SSG)

| Aspecto | CMS Dinámico | Generador Estático |
| :--- | :--- | :--- |
| **Forma de crear contenidos** | A través de un panel de administración visual (dashboard) con editores WYSIWYG o bloques | Redactando archivos de texto plano (principalmente en formato Markdown) en un editor de código |
| **Base de datos** | Sí (utiliza bases de datos relacionales como MySQL o PostgreSQL para consultar el contenido) | No (el contenido reside directamente en el sistema de archivos del proyecto) |
| **Generación del HTML** | En tiempo real / bajo demanda (se compila dinámicamente cada vez que un usuario solicita la página) | Por adelantado (se compila durante la fase de build o desarrollo, previo a la publicación) |
| **Servidor necesario** | Servidor de aplicaciones activo que ejecute un lenguaje backend (PHP, Node.js, Python, etc.) y la base de datos | Servidor web simple o CDN (Content Delivery Network) para entregar archivos estáticos |
| **Panel de administración** | Sí, integrado de forma nativa para gestionar la web visualmente sin tocar código | No por defecto (opcionalmente se puede integrar un Headless CMS o CMS basado en Git) |
| **Conocimientos técnicos** | Bajos para el usuario/creador de contenido; medio-altos solo para el mantenimiento o desarrollo inicial | Medios a altos (requiere uso de la consola/terminal, Git y sintaxis de motores de plantillas) |
| **Seguridad** | Menor (al estar expuesto a bases de datos y backend, es más susceptible a inyecciones SQL, vulnerabilidades en plugins y ataques de fuerza bruta) | Alta (al no tener base de datos ni procesamiento en servidor en tiempo real, la superficie de ataque es mínima) |
| **Rendimiento** | Variable / Menor (requiere procesamiento en servidor y consultas a la BD, aunque se mitigue con sistemas de caché) | Máximo (la carga es casi instantánea al servir archivos HTML directos desde una CDN) |
| **Actualización del contenido** | Inmediata; los cambios guardados en el panel se reflejan instantáneamente al recargar la página | Requiere recompilación (rebuild); es necesario regenerar el proyecto y subir los archivos actualizados al servidor |
| **Publicación** | Se guarda el cambio en el panel y la base de datos lo sirve en tiempo real | Se hace un build del proyecto y se despliega la carpeta de salida a un servicio de hosting o CDN (vía Git/CI-CD) |
| **Ejemplos** | WordPress, Joomla, Drupal, PrestaShop | Jekyll, Hugo, Astro, Eleventy, Gatsby |

### Video explicativo CMS
([CMS](https://www.youtube.com/watch?v=OBJP4dvoS_I))

### enlace a la siguiente página SSG
**[Ver documento sobre Generadores de Sitios Estáticos (ssg.md)](ssg.md)**