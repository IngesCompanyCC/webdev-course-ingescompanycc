# Lección 3: Listas, imágenes y enlaces

_(Contenido para los instructores)_

**Objetivo:** Al terminar, el estudiante puede agregar a su página una lista con viñetas, una lista numerada, una imagen con su texto alternativo y un enlace que abre en una pestaña nueva.

**Palabras nuevas:** lista, viñeta, imagen, atributo `src`, texto alternativo (`alt`), enlace, atributo `href`, pestaña nueva.

## 1. Estructura de carpetas (GitHub)

```text
/starter-files/leccion-03        # Código de inicio de la lección
└── index.html

/completed-examples/leccion-03   # Código completo de la lección
└── index.html

/starter-files/assets            # Imagen de la lección (se enlaza con su dirección completa)
└── avatar.png
```

## 2. Guion del video (10 minutos)

> Los tiempos son los del audio (unos 8:57). Con las tarjetas de pausa, los Ejecutar y las transiciones de la edición, el video llega a unos 10 minutos. El guion detallado para grabar está en `grabacion/leccion-03.md` (solo para el equipo).

> **(0:00 - 0:46) Introducción**  
> ¡Hola! Te doy la bienvenida a la lección 3. Ya sabes escribir títulos y párrafos. Hoy vas a darle más vida a tu página con tres cosas que usarás siempre: listas, imágenes y enlaces. Piensa en tu app favorita: tiene listas de publicaciones, fotos por todas partes y enlaces que te llevan a otras páginas. ¡Hoy aprendes a hacer las tres! Al final, tu página va a tener tus pasatiempos en una lista, tus metas numeradas, tu foto y un enlace a tu sitio favorito.
>
> **(0:46 - 2:04) Listas con viñetas**  
> Aquí está la página de la lección anterior. Empecemos por las listas. Están en todas partes: tu lista de canciones, el menú de un restaurante o los ajustes de tu celular. Voy a cambiar el párrafo de mis pasatiempos por una lista. Una lista no ordenada, con viñetas, se escribe con la etiqueta u l. Adentro, cada elemento va en su propia etiqueta l i: Dibujar, Jugar fútbol y Escuchar música. Ejecutar. ¡Mira! Aparecen mis pasatiempos, cada uno con su viñeta, ese puntito del inicio. u l viene de unordered list, lista no ordenada; y l i, de list item, elemento de la lista. Fíjate en la sangría: los l i van un poco más adentro que el u l, así se ve qué está dentro de qué.
>
> **(2:04 - 3:07) Listas numeradas**  
> Cuando el orden importa, se usa una lista ordenada, con la etiqueta o l. Sirve para rankings, como el top 3 de tus videojuegos, o para los pasos de un tutorial. Debajo escribo un subtítulo, Mis 3 metas del año, y una lista o l con tres metas: Aprender HTML y CSS, Mejorar mis dibujos e Ir a un concierto. Ejecutar. Los elementos son los mismos, l i, pero ahora el navegador los numera por nosotros. Prueba rápida: muevo Ir a un concierto al primer lugar y pulso Ejecutar. ¡Los números se ajustan solos! Lo regreso a su lugar con Control Z.
>
> **(3:07 - 3:43) ¿Viñetas o números?**  
> ¿Cuál elegir? Depende de si el orden importa. Los ingredientes de una receta van en una lista no ordenada, porque no importa cuál compras primero. Los pasos van en una lista ordenada, porque no puedes hornear el pastel antes de mezclar la masa. Otro ejemplo: tu lista de reproducción puede ir con viñetas, pero el ranking de tus canciones más escuchadas va con números.
>
> **(3:43 - 4:59) Imágenes**  
> Ahora una imagen, con la etiqueta i m g. Esta etiqueta no necesita cierre, porque no tiene contenido adentro. Usa dos atributos importantes. src dice dónde está la imagen: es su dirección. alt es un texto que describe lo que se ve. Lo usan las personas que escuchan la página con un lector de pantalla, y también aparece cuando la imagen no carga. Debajo del título escribo img, el src con la dirección de la imagen, el alt, Dibujo de Alex sonriendo con audífonos, y width igual a 200, que es el ancho en píxeles. Ejecutar. ¡Ahí está el dibujo de Alex! Prueba rápida: cambio el 200 por 100 y pulso Ejecutar. La imagen se achica. La regreso a 200 y pulso Ejecutar.
>
> **(4:59 - 5:43) Cuando la imagen no carga**  
> Voy a equivocarme a propósito. En la dirección borro una letra: avatr en vez de avatar. Ejecutar. La imagen no carga, pero mira: aparece el texto alternativo. Por eso nunca lo dejes vacío; también lo usan los buscadores para saber qué hay en la imagen. Corrijo la letra, pulso Ejecutar y la imagen vuelve. Y un consejo: usa solo imágenes que sean tuyas o que tengan permiso para usarse, y no publiques fotos de otras personas sin su permiso.
>
> **(5:43 - 6:48) Enlaces**  
> Y llegamos a los enlaces, que son los que convierten un conjunto de páginas en un sitio web. Se escriben con la etiqueta a. Al final de la página escribo un párrafo, Mi sitio favorito para aprender, y adentro el enlace. El atributo href dice adónde lleva: la dirección de MDN Web Docs. Y el texto de en medio es lo que se ve y lo que se toca. Un enlace puede llevar a otro sitio, como este, o a otra página de tu propio sitio: así se conectan las páginas, como viste en la lección 1. Ejecutar. ¡El enlace aparece en azul y subrayado! Enseguida lo probamos.
>
> **(6:48 - 7:32) Enlaces en una pestaña nueva**  
> Si quieres que el enlace abra en una pestaña nueva, agrega target igual a guion bajo blank. Y suma rel igual a noopener, una buena costumbre de seguridad cuando abres una pestaña nueva. Ejecutar. Hago clic y… ¡MDN se abre en otra pestaña, y mi página sigue aquí! Así quien visita tu página no la pierde, como cuando abres un video desde un chat y el chat sigue ahí.
>
> **(7:32 - 8:02) Antes de publicar**  
> Un aviso importante antes de seguir. Las páginas que haces en un editor en línea pueden verse en internet. Nunca escribas en ellas tu dirección, tu teléfono, tu apellido ni el nombre de tu colegio. Usa un apodo, y comparte solo lo que te sentirías cómodo de que vea cualquier persona.
>
> **(8:02 - 8:30) Pausa y prueba**  
> ¡Te toca! Pausa el video y abre el enlace de la descripción. Agrega a tu página una lista con tus pasatiempos, una lista numerada con tus metas y un enlace a tu sitio favorito. Si quieres poner una imagen, recuerda escribir su texto alternativo. Cuando termines, sigue con el video.
>
> **(8:30 - 8:57) Resumen**  
> ¡Excelente! Tu página ya tiene mucho contenido. Hoy aprendiste a crear listas con viñetas y numeradas, a poner imágenes con su texto alternativo y a crear enlaces, incluso en una pestaña nueva. En la próxima lección empezamos con CSS, para darle color y estilo a tu página. ¡Nos vemos ahí!

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 14:** Lámina de título. Sin texto añadido en pantalla.
- **Listas con viñetas (0:46), Editor (JSFiddle), sin lámina:** JSFiddle con el fiddle de inicio (título, subtítulo y dos párrafos). El párrafo de pasatiempos se reemplaza por un `<ul>` con tres `<li>`: Dibujar, Jugar fútbol y Escuchar música; se pulsa Ejecutar. Texto en pantalla: «`ul` = lista con viñetas (unordered list)» · «`li` = cada elemento (list item)». Anotación: llave sobre `ul` que abarca los `li`.
- **Listas numeradas (2:04), Editor (JSFiddle), sin lámina:** Debajo de la primera lista se escriben `<h2>Mis 3 metas del año</h2>` y un `<ol>` con tres metas, y se pulsa Ejecutar. Prueba rápida: la última meta sube al primer lugar, se pulsa Ejecutar (los números se ajustan) y se deshace con `Ctrl + Z`. Texto en pantalla: «`ol` = lista numerada» · «¿Importa el orden? Usa `ol`».
- **¿Viñetas o números? (3:07), Lámina 15:** Lámina con dos columnas: «Ingredientes» (`ul`, lista no ordenada) y «Pasos» (`ol`, lista ordenada). Sin texto añadido en pantalla.
- **Imágenes (3:43), Lámina 16 (unos 5 s) y luego el editor (JSFiddle):** Primero la Lámina 16, con las etiquetas `img` y `a`. Luego, debajo del `h1`, se escribe `<img src="…/avatar.png" alt="Dibujo de Alex sonriendo con audífonos" width="200">` (con la dirección completa) y se pulsa Ejecutar: aparece la imagen. Prueba rápida con `width="100"` y vuelta a 200. Texto en pantalla (solo durante el editor): «`img` no necesita cierre» · «`width` = ancho en píxeles». Anotación: subrayar `src` y `alt`.
- **Cuando la imagen no carga (4:59), Editor (JSFiddle), sin lámina:** En el `src` se borra una letra (`avatr.png`) y se pulsa Ejecutar: la imagen no carga y aparece el texto `alt`. Luego se corrige y se pulsa Ejecutar. Texto en pantalla: «Si la imagen no carga, aparece el `alt`». Anotación: círculo sobre el texto alternativo.
- **Enlaces (5:43), Editor (JSFiddle), sin lámina:** Al final se escribe el párrafo `<p>Mi sitio favorito para aprender:` con `<a href="https://developer.mozilla.org/es/">MDN Web Docs</a>` adentro, y se pulsa Ejecutar. Todavía no se hace clic. Texto en pantalla: «`a` = enlace» · «`href` = adónde lleva». Anotación: flecha de `href` al texto del enlace.
- **Enlaces en una pestaña nueva (6:48), Editor (JSFiddle), sin lámina:** Dentro de la etiqueta `a`, después del `href`, se agrega `target="_blank" rel="noopener"` y se pulsa Ejecutar. Al hacer clic, MDN se abre en una pestaña nueva; se cierra y se vuelve a JSFiddle. Texto en pantalla: «`target="_blank"` = pestaña nueva» · «`rel="noopener"` = buena costumbre de seguridad».
- **Antes de publicar (7:32), Lámina 17:** Lámina «Antes de publicar», con una tarjeta de perfil y un ojo tachado: nunca publicar la dirección, el teléfono, el apellido ni el colegio. Sin texto añadido en pantalla.
- **Pausa y prueba (8:02), Lámina 18:** Tarjeta de pausa de 5 segundos. Sin texto añadido en pantalla.
- **Resumen (8:30), Lámina 19:** Lámina de resumen con tres tarjetas. Sin texto añadido en pantalla.

## 4. Pregunta para pensar

¿por qué es mejor escribir «Dibujo de Alex sonriendo con audífonos» que dejar el `alt` vacío o poner «imagen»?
