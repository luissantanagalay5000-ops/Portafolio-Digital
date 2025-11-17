# Portafolio-Digital
Acerca De Mi

Se han proporcionado tres archivos (Style.css, index.html, y mobile.css) que definen la estructura y el estilo de una página web de Portafolio Digital. A continuación, se detalla lo que se hizo en cada uno de ellos.

1. Archivo index.html (Estructura de la Página)
Este archivo define la estructura (esqueleto) de la página web utilizando HTML5.

Encabezado (<head>)
Establece la codificación de caracteres (UTF-8) y la configuración de la vista móvil (viewport).

Vincula los archivos de estilos CSS:

Style.css: Contiene los estilos base o principales.

mobile.css: Contiene los estilos que se aplican específicamente cuando la pantalla tiene un ancho máximo de 768px (diseño responsive).

Define el título de la página como "Portafolio Digital".

Cuerpo (<body>)
Header (<header id="mainheader">)

Barra de Navegación (<nav id="navbar">):

Contiene el logo (un <a> con una imagen <img> vacía).

Define una lista no ordenada (<ul>) de enlaces de navegación que apuntan a diferentes secciones de la página (Proyectos, Acerca De, Contactos).

Sección de Presentación (<div id="showcase">):

Contiene un botón con la clase btn btn-outline que, aunque está en el código, aparece vacío en el HTML. Su función es probablemente llevar a la sección de Proyectos.

Secciones Principales (<section>)

Proyectos (<section id="proyecto">):

Título: "Portafolio" (<h2>).

Contiene un div con una imagen (<img>) dentro, presumiblemente para mostrar el detalle de un proyecto.

Acerca de (<section id="Acerca_de">):

Título: "Acerca de" (<h2>).

Estructura dividida en dos partes:

Experiencias: Lista de experiencias laborales o roles con títulos y años.

Acerca de mí: Párrafo de presentación personal que incluye nombre, edad, lugar de nacimiento, y detalles de su matrícula en la universidad O&M (Ing. Sistemas y Computación).

Contactos (<section id="Contactos">):

Estructura de fila (Contactos-row) con tres columnas (Contactos-row-icono) para mostrar información de contacto:

Ubicación (Av. Santa Rosa 196) con un ícono.

Correo electrónico (dionismetivier@gmail.com) con un ícono.

Teléfono (849-388-4249) con un ícono.

Footer (<footer id="mainfooter">)

Contiene un botón de seguimiento de Instagram (instagram-Boton-Seguir) que enlaza al perfil @333_dionis e incluye el logo de Instagram.

2. Archivo Style.css (Estilos Base)
Este archivo contiene los estilos generales y el diseño para pantallas de escritorio (tamaños grandes), utilizando una tipografía de Google Fonts, 'Poppins'.

Configuración Base
Importación de Fuente: Se importa la fuente 'Poppins' de Google Fonts.

Reinicio (*): Se eliminan los márgenes y paddings predeterminados y se establece box-sizing: border-box para un manejo más predecible del tamaño de los elementos.

Estilo Tipográfico:

La fuente base es 'Poppins' para html y body.

Se definen tamaños y pesos para títulos (h2, h4) y párrafos (p).

Se eliminan las decoraciones de los enlaces (a).

Clases de Utilidad:

.container: Centra el contenido, establece un ancho máximo de 1100px y maneja el overflow.

.large: Aumenta el tamaño de la fuente a 20px.

.btn y .btn-outline: Clases para estilizar botones con un diseño "contorneado" (borde) en blanco, fondo transparente, y efecto hover que invierte los colores.

Diseño de Secciones
Barra de Navegación (#navbar):

Usa float: left y float: right para posicionar el logo a la izquierda y los enlaces a la derecha.

Los elementos de la lista (<li>) se colocan en línea (float: left).

Presentación (#Presentacion):

Establece una imagen de fondo (descarga-_45_.jpg), centrada y cubriendo todo el contenedor.

Define una altura fija de 500px y centra el texto.

El botón de esta sección tiene un gran margen superior (margin-top: 250px).

Proyectos (#Proyectos):

Usa Flexbox (display: flex) para alinear los detalles de los proyectos.

Acerca de (#Acerca_de):

Usa Flexbox para la disposición de los detalles (Acerca_de-detalles).

Divide la sección de Experiencias y Acerca de mí en dos columnas, cada una tomando el 50% del ancho.

Contactos (#Contactos):

Usa Flexbox para la fila (Contactos-row), dividiendo los íconos de contacto en tres columnas (33% de ancho cada una).

Footer (#mainfooter):

Estilos para el botón de seguimiento de Instagram: lo hace inline-flex, le da un borde, padding, e invierte el color de la imagen del ícono (filter: invert(1)). Define un efecto hover con fondo oscuro.

3. Archivo mobile.css (Estilos para Móviles)
Este archivo utiliza Media Queries implícitas (ya que está vinculado con media="screen and (max-width:768px)" en el HTML) para reestructurar el diseño, optimizándolo para pantallas pequeñas (máximo 768px de ancho).

Ajustes Principales
Padding Reducido: El padding vertical de las secciones Proyectos, Acerca de, y Contactos se reduce a 50px para aprovechar mejor el espacio vertical en móviles.

Acerca de (#Acerca_de):

Se utiliza Flexbox con flex-wrap: wrap para que las columnas de Experiencias y Acerca de mí se apilen verticalmente en lugar de estar una al lado de la otra.

Ambas subsecciones ahora ocupan el 100% del ancho disponible y se elimina el padding izquierdo.

Se centraliza el texto de los párrafos y títulos h4 (aunque la regla para h4 está mal anidada en el código CSS, su intención es clara).

Contactos (#Contactos):

Se reduce ligeramente el tamaño de fuente de los párrafos a 14px para ahorrar espacio.
