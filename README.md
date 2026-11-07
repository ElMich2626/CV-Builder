# CV Builder

Plantilla HTML y CSS para crear currículums vitae personalizados y exportarlos a PDF desde un navegador web. El proyecto ofrece dos estilos base de presentación: uno optimizado para sistemas de seguimiento de candidatos (ATS) y otro orientado a una presentación visual para lectura e impresión.

## Contenido del proyecto

- `Plantilla.html`: plantilla HTML que contiene la estructura y los campos que se deben completar con la información personal y profesional.
- `CV-ATS.css`: hoja de estilos sencilla, pensada para facilitar la lectura y extracción de información por sistemas ATS.
- `CV-Imprimir.css`: hoja de estilos con diseño visual de dos columnas, colores y códigos QR para determinados enlaces.
- `Demostracion.html`: ejemplo de una plantilla completada para mostrar el resultado.

## Cómo utilizarlo

### 1. Completar la plantilla HTML

1. Abrí `Plantilla.html` con un editor de texto o de código, como Visual Studio Code.
2. Reemplazá los campos indicados entre corchetes (`[ ... ]`) por tu propia información.
3. Completá las secciones que correspondan a tu perfil:
   - Nombre y perfil profesional.
   - Datos de contacto.
   - Experiencia profesional.
   - Educación.
   - Cursos y certificaciones.
   - Idiomas.
   - Habilidades técnicas y blandas.
4. Si necesitás agregar experiencias, estudios, cursos, idiomas o enlaces, seguí las indicaciones incluidas en los comentarios de la plantilla.
5. Eliminá las secciones o elementos de ejemplo que no correspondan a tu situación.

**Enlaces y códigos QR:** para generar un código QR junto a un enlace, conservá el atributo `data-qr="true"` y reemplazá su dirección por una URL válida. La plantilla permite utilizarlo en enlaces de contacto, perfiles y certificados.

### 2. Seleccionar el diseño CSS

En la sección `<head>` de `Plantilla.html`, buscá la siguiente línea:

```html
<link rel="stylesheet" href="[ARCHIVO-CSS]" />
```

Reemplazá `[ARCHIVO-CSS]` por el nombre del archivo CSS que quieras utilizar:

- Para el formato ATS:

  ```html
  <link rel="stylesheet" href="CV-ATS.css" />
  ```

- Para el formato visual de impresión:

  ```html
  <link rel="stylesheet" href="CV-Imprimir.css" />
  ```

Los archivos HTML y CSS deben permanecer en la misma carpeta, salvo que modifiques la ruta indicada en `href`.

### 3. Abrir el currículum en el navegador

Guardá los cambios y abrí `Plantilla.html` con tu navegador de preferencia, por ejemplo, Google Chrome, Microsoft Edge o Mozilla Firefox.

Revisá que la información esté completa y que el diseño se muestre correctamente. Si modificás el archivo HTML o CSS, guardá los cambios y actualizá la página del navegador.

### 4. Exportar el currículum a PDF

1. Con el currículum abierto en el navegador, utilizá la opción **Imprimir** (`Ctrl + P`).
2. En el apartado de destino o impresora, seleccioná **Guardar como PDF** o la opción equivalente.
3. Comprobá el tamaño de papel y la vista previa.
4. Si utilizás `CV-Imprimir.css`, habilitá **Gráficos de fondo** para conservar los colores y elementos visuales del diseño.
5. Seleccioná **Guardar** y elegí la ubicación del archivo PDF.

El resultado será un documento PDF listo para compartir o adjuntar en una postulación.

## Consideraciones

- **Conexión a Internet:** la plantilla carga la biblioteca QRCode.js desde un CDN para generar los códigos QR. El diseño de impresión también utiliza recursos externos para algunos iconos. Por eso, se recomienda contar con conexión a Internet al abrir el HTML y generar el PDF.
- **Diseño ATS:** `CV-ATS.css` oculta los códigos QR y utiliza un formato más simple.
- **Diseño de impresión:** `CV-Imprimir.css` muestra los códigos QR y aplica el diseño visual de dos columnas.
- **Mantenimiento:** para personalizar la apariencia, modificá los archivos CSS sin alterar innecesariamente la estructura HTML de la plantilla.

## Desarrollo asistido por IA

Este proyecto fue desarrollado con asistencia de inteligencia artificial.

Las decisiones sobre el funcionamiento, la estructura y las características del proyecto fueron definidas durante el proceso de desarrollo, con revisión y validación de los resultados.

## Tecnologías utilizadas

- **HTML5:** estructura y contenido de la plantilla.
- **CSS3:** diseño y estilos de presentación.
- **JavaScript:** generación automática de códigos QR.

### Bibliotecas y recursos externos

- [QRCode.js](https://github.com/davidshimjs/qrcodejs) (1.0.0): generación de códigos QR. Licencia MIT.
- [Font Awesome Free](https://fontawesome.com/) (6.7.2): iconos de contacto. Licencia CC BY 4.0 para los iconos SVG utilizados.
- [Simple Icons](https://simpleicons.org/) (v16): icono de GitHub. Consultar la licencia individual del icono.

## Créditos

CV Builder utiliza bibliotecas y recursos gráficos de terceros.
Se reconocen sus respectivos autores y se respetan las licencias
correspondientes. Los créditos de estos recursos son independientes
de la licencia principal del proyecto.

## Licencia

Este proyecto se distribuye bajo la licencia [MIT](LICENSE).

Esto permite utilizar, copiar, modificar y distribuir el proyecto,
incluso con fines comerciales, siempre que se conserve el aviso de
copyright y el texto de la licencia en las copias o partes sustanciales
del software.

La licencia se aplica a CV Builder y no reemplaza las licencias
individuales de las bibliotecas y recursos de terceros utilizados.