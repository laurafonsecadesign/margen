# MARGEN. — Decisiones de diseño

**Laura Fonseca · Proyecto universitario de HTML y CSS · Octubre de 2026**

## 01 / Concepto de la revista

### Una invitación a mirar otra vez

MARGEN es una revista digital sobre diseño, arte y cultura visual. La idea es hablar de elementos que vemos todos los días, pero a los que muchas veces no prestamos demasiada atención: una letra, un cartel, un objeto o una composición. El nombre hace referencia a lo que queda alrededor de una página y, al mismo tiempo, a las cosas que suelen pasar desapercibidas.

Quería que tuviera una personalidad editorial, parecida a la de una revista impresa, sin dejar de ser una web fácil de recorrer.

### A quién va dirigida

Está pensada principalmente para estudiantes, personas creativas y lectores con interés por la cultura visual. Por eso los textos son cercanos y no dan por hecho que todo el mundo conozca vocabulario técnico de diseño. La navegación permite entrar por tres categorías y descubrir artículos completos a partir de ellas.

## 02 / Identidad visual

### Colores y tipografía

La identidad se construye con una paleta reducida. El color principal es el rojo **#FF5A5B**, acompañado del granate **#570000**. Para las zonas de lectura se utiliza el tono papel **#E8E3DC**. Los textos y detalles secundarios usan **#292423**, **#57514E** y **#B8AFA7**. Los mismos colores se repiten en las páginas interiores para mantener una relación con la portada.

La tipografía principal es **Switzer**. Los titulares llevan Switzer Regular, normalmente en mayúsculas, con un interletrado de -5 %. Los párrafos y la información más pequeña usan Switzer Light, con un espaciado más natural para leer cómodamente. El rótulo MARGEN se utiliza también como un SVG para conservar la forma del diseño original.

La palabra **Fuera** en el manifiesto de la home tiene un tratamiento distinto. La fuente preferida es ITC Legacy Sans Std Medium Italic, pero no se incluye su archivo comercial en el proyecto. Si el navegador no la tiene, se usa una versión local de Switzer Italic como alternativa. Además, el peso Light de Switzer se carga desde Fontshare, así que para reproducirlo exactamente es necesaria una conexión a Internet.

### Composición e imágenes

Tomé como punto de partida el diseño de la home en Figma. Mantuve la portada roja, el logotipo a gran escala y la combinación de titulares grandes con bloques de texto más tranquilos. En las páginas interiores cambié algunas distribuciones, pero conservé los márgenes, las líneas divisorias, los colores y la jerarquía.

La revista utiliza fotografías para algunas historias y gráficos SVG para otras. Las ilustraciones acompañan el tema de cada artículo, no son solo decoración. Las fuentes de las fotos y de la tipografía están recogidas en **creditos.html**.

## 03 / Estructura de la web

### Trece páginas conectadas

El proyecto tiene una home, tres categorías (Diseño, Arte y Cultura), las páginas About y Créditos y siete artículos. Cada categoría reúne sus publicaciones. Desde las tarjetas se puede abrir el artículo completo y desde los artículos se puede volver a la sección correspondiente o seguir leyendo.

La home funciona como portada de la revista. Presenta el artículo destacado, las últimas publicaciones, el acceso a categorías y un pequeño manifiesto. En los artículos he priorizado una columna de lectura con títulos, entradillas, imágenes y subtítulos.

### Retícula y responsive

He utilizado **CSS Grid** para las tarjetas y otros bloques de varias columnas, y **Flexbox** para la navegación y los elementos que necesitan alinearse en una fila. La hoja de estilos tiene media queries para adaptar tamaños y distribución.

En escritorio las composiciones dejan más espacio a las imágenes y los titulares. En móvil el contenido se ordena verticalmente y la navegación pasa a un menú a pantalla completa. Este menú funciona con un checkbox de HTML y transiciones CSS. Los enlaces aparecen de forma escalonada al abrirlo, sin necesitar JavaScript.

### Interacciones

Los enlaces tienen estados hover y de foco para indicar que se pueden pulsar. Hay algunas animaciones suaves de entrada y una frase en movimiento en la home. El CSS incluye una opción para reducir estas animaciones cuando el usuario tiene activada la preferencia de movimiento reducido.

## 04 / Desarrollo

### HTML y CSS

He organizado el contenido en archivos HTML separados y he utilizado una sola hoja **css/style.css** para los estilos comunes. El CSS está dividido por secciones comentadas: fuentes y base, navegación, home, páginas interiores, responsive y animaciones.

He usado etiquetas como **header**, **nav**, **main**, **section**, **article** y **footer** para separar el contenido de manera clara. Todas las páginas tienen un H1 principal, una descripción y un enlace para saltar al contenido. Las imágenes HTML llevan texto alternativo.

No he utilizado frameworks ni JavaScript. El proyecto se puede abrir desde **index.html** después de descomprimir la carpeta, aunque algunos recursos tipográficos dependen de Internet.

### Archivos y recursos

Las fotografías y los SVG están en **assets/images/**. Los archivos locales de Switzer y su licencia se encuentran en **assets/fonts/**. Las rutas son relativas, por lo que la estructura funciona al mover la carpeta completa a otro ordenador.

## 05 / Revisión de la entrega

He comprobado las trece páginas HTML: todas contienen un elemento main y un H1, no tienen imágenes HTML sin atributo alt y sus rutas internas apuntan a archivos existentes. También he comprobado los enlaces con anclas y las referencias locales desde el CSS.

La comprobación automática de archivos no sustituye a la revisión visual. Antes de la entrega final conviene abrir la web en el navegador, probarla en un ancho de escritorio y otro de móvil, abrir y cerrar el menú y comprobar los textos y las imágenes.

## Referencias

- **Diseño original en Figma:** https://www.figma.com/design/auIdICJ4fPgWbjJy12P4h6/Untitled?node-id=8-3
- **Switzer / Fontshare:** https://www.fontshare.com/fonts/switzer
- **Licencia de fotografías Unsplash:** https://unsplash.com/license
- **Créditos de imágenes y tipografía:** creditos.html
- **Web publicada:** https://laurafonsecadesign.github.io/margen/
