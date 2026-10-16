# MARGEN. — Decisiones de diseño

Laura Fonseca · Proyecto académico HTML y CSS · Octubre 2026

## 01 / CONCEPTO E IDENTIDAD

### Una revista para mirar dos veces

MARGEN es una revista digital en español sobre diseño, arte y cultura visual. Está pensada para estudiantes y personas interesadas en la creatividad. El nombre conecta los márgenes de una página con la idea de observar aquello que suele quedar fuera del foco.

### De Figma a la web

La home facilitada en Figma define la dirección visual: una portada roja, el rótulo MARGEN a gran escala, un artículo destacado, tarjetas, categorías, una cita y un manifiesto. Se mantiene ese orden. La etiqueta técnica del wireframe no forma parte de la web.

### Color y tipografía

La paleta procede de la home: rojo #FD3738, granate #570000, fondo cálido #DBD5CE y texto #292423. Switzer sustituye a Inter en todo el texto HTML, con interlineado del 90% y espaciado entre letras de -5%. Los rótulos MARGEN y EXPLORA conservan sus vectores originales.

### Imagen y tono

Se combinan fotografías de arte urbano, arquitectura y cerámica con composiciones gráficas editoriales. Los textos son cercanos y reflexivos, sin presentarse como noticias o entrevistas. Los créditos distinguen las fotografías de los gráficos preparados para el proyecto.

## 02 / ESTRUCTURA Y EXPERIENCIA

### Arquitectura de contenidos

La revista tiene 13 páginas: Inicio, Diseño, Arte, Cultura, About, Créditos y siete artículos. Cada categoría reúne sus contenidos. Todas las tarjetas enlazan a artículos completos; el principal, «Cuando el diseño deja de ser perfecto», tiene 443 palabras.

### Un sistema compartido

Todas las páginas repiten cabecera, navegación, colores, tipografía y pie. Las categorías utilizan títulos grandes y una cuadrícula de tarjetas. Los artículos tienen titular, entradilla, imagen, crédito, texto por apartados y lecturas relacionadas. About desarrolla el manifiesto de la home.

### Distribución responsive

CSS Grid organiza las tarjetas y el destacado; Flexbox distribuye la navegación y otros elementos. En pantallas grandes hay tres columnas. A 1000 px se reducen márgenes y espacios. A 700 px la composición pasa a una columna y el menú queda visible, sin depender de JavaScript.

### Semántica y accesibilidad

Se utilizan header, nav, main, section, article y footer. Cada página tiene un H1 y una jerarquía de subtítulos. Las imágenes llevan texto alternativo; el documento declara lang="es". Se incluyen foco visible, un enlace para saltar al contenido y soporte para movimiento reducido.

## 03 / DESARROLLO Y ENTREGA

### HTML y CSS sencillos

La web es estática y no necesita frameworks, JavaScript ni instalación. Los HTML son independientes y comparten css/style.css, dividida en bloques comentados. Se emplean clases descriptivas como cabecera, tarjeta, destacado y lectura para facilitar la edición.

### Recursos locales

Las imágenes y Switzer se guardan en assets. Las rutas son relativas, de modo que el proyecto puede abrirse desde index.html al descomprimirlo. Se usan SVG para los rótulos y composiciones, JPG para las fotografías y WOFF2 para las fuentes. Se adjunta la licencia oficial de Switzer.

### Interacción y navegación

Los controles son enlaces con destinos reales. Hay acceso a las categorías desde el menú y desde EXPLORA, retorno desde los artículos y un enlace para subir al inicio. Los estados hover ofrecen respuesta visual; el sitio mantiene su funcionamiento sin animación.

### Referencias y revisión

El diseño de referencia es la home de Figma proporcionada para MARGEN. Switzer procede de Fontshare; las fotografías, de Unsplash, con fuentes enlazadas en Créditos. Se han verificado las 354 referencias locales, la jerarquía principal y los recursos. Queda pendiente la revisión visual en navegador antes de la entrega.

## Fuentes

- Home: https://www.figma.com/design/auIdICJ4fPgWbjJy12P4h6/Untitled?node-id=8-3
- Tipografía: https://www.fontshare.com/fonts/switzer
- Fotografía y licencia: https://unsplash.com/license
- Fuentes individuales: página creditos.html de la web.
