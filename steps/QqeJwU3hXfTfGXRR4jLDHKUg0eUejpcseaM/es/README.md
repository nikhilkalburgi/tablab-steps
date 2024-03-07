# Formato de redacción a seguir y restricciones de derechos de autor

* Crear un Step en [tablab.io][1] consiste en ofrecer una experiencia de aprendizaje concisa, clara y atractiva. Esta guía se centra en el formato y el estilo de redacción esenciales para crear un Step eficaz.

## Sigue nuestra convención de estilo de escritura

* Utiliza la sintaxis Markdown para dar estilo a todos los escritos.
* Describa los conceptos mediante listas de enumeración con frases cortas y concretas, como esta.

### Uso de emojis

* :writing_hand: (`:writing_hand:`): se utiliza para indicar al lector que a continuación se encuentra un ejercicio práctico.
* :older_man: (`:older_man:`): se utiliza para explicar algún concepto relacionado con el Step el cual no se trata específicamente.
* :warning: (`:warning:`): se utiliza cuando es aconsejable que el lector preste atención a una sección importante.

### Añadir una tabla

* Puedes añadir tablas cuando sea necesario. Para ello, ten en cuenta que este es el formato que procesa nuestro renderizador de Markdown:

  ```markdown
  |Column 1|Column 2|Column 3|
  |:--:|:--:|:--:|
  |Field 1|Field 2|Field 3|
  |Field 4|Field 5|Field 6|
  ```

### Añadir una imagen

* Cuando quieras añadir una imagen al contenido para explicar un concepto de forma más representativa, primero necesitas obtener la imagen en tu ordenador y luego colocarla como archivo estático en la carpeta `/static/images/` que encontrarás en este repositorio.
* Una vez hecho esto, puedes incrustar la imagen siguiendo el código Markdown como se muestra:

  ```markdown
  ![Image caption here][1]
  ```

  Después, solo tienes que hacer referencia a la imagen al final del archivo de la siguiente forma:

  ```markdown
  [1]: /static/images/your-selected-image.png
  ```

  Ten en cuenta que la ruta de la imagen `/static/images/your-selected-image.png` se refiere a la ruta absoluta donde supuestamente se ha colocado la imagen en este repositorio.
* **Notificación importante**: puedes añadir cualquier imagen que desees, aunque no la hayas creado tú mismo. Nosotros nos encargaremos de crear una nueva imagen que represente exactamente el mismo concepto pero en formato corporativo (estilos y colores) y evitando cualquier infracción de derechos de autor.

### Uso de Visual Studio Code

* Aquellos que utilicen Visual Studio Code encontrarán en este mismo repositorio configuraciones para varios plugins diseñados para mejorar su experiencia de escritura en Markdown.
* Para instalar las extensiones recomendadas para este proyecto, sigue estos pasos en Visual Studio Code:
  1. Inicia Visual Studio Code cargando el repositorio [tablab-steps][2].
  1. Navega a la vista de *Extensions* pulsando `Ctrl+Shift+X` (o `Cmd+Shift+X` en macOS).
  1. Escribe `@recommended` en la barra de búsqueda.
  1. Haz clic en el botón de instalación situado junto a las extensiones enumeradas en *Workspace Recommendations*.

## Respeta los derechos de autor

* Como creador de contenido, es fundamental comprender y respetar las leyes de derechos de autor, asegurándote de no utilizar ni replicar frases o textos de otros sitios web.
* El mero intercambio de palabras con significados similares en una frase, sin modificar la estructura de la misma ni la gramática, sigue considerándose una forma de plagio.
* Las herramientas de IA pueden ayudarte en la creación de contenido, pero no se permiten textos producidos directamente por sistemas de inteligencia artificial en [tablab.io][1].

[1]: https://tablab.io
[2]: https://github.com/samus-io/tablab-steps
