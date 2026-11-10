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

> **(0:00 - 0:30) Introducción**  
> Ya sabes escribir títulos y párrafos. Hoy vas a darle más vida a tu página con tres cosas que usarás siempre: listas, imágenes y enlaces.
>
> **(0:30 - 2:00) Listas con viñetas**  
> Empecemos por las listas. Voy a cambiar el párrafo de mis pasatiempos por una lista. Una lista no ordenada, con viñetas, se escribe con la etiqueta u l. Adentro, cada elemento va en una etiqueta l i. Mira el resultado: aparecen mis pasatiempos, cada uno con su viñeta. Cada elemento va en su propia etiqueta.
>
> **(2:00 - 3:00) Listas numeradas**  
> Cuando el orden importa, se usa una lista ordenada, con la etiqueta o l. Los elementos son los mismos, l i, pero ahora el navegador los numera por nosotros. Si cambio el orden de las metas, los números se ajustan solos.
>
> **(3:00 - 3:30) ¿Viñetas o números?**  
> ¿Cuál elegir? Depende de si el orden importa. Los ingredientes de una receta van en una lista no ordenada, porque no importa cuál va primero. Los pasos van en una lista ordenada, porque sí importa el orden.
>
> **(3:30 - 5:00) Imágenes**  
> Ahora una imagen, con la etiqueta i m g. Fíjate: esta etiqueta no necesita cierre, porque no tiene contenido adentro. Usa dos atributos importantes. `src` dice dónde está la imagen: es su dirección. `alt` es un texto que describe lo que se ve. Lo usan las personas que escuchan la página con un lector de pantalla y también aparece cuando la imagen no carga.
>
> **(5:00 - 6:15) Cuando la imagen no carga**  
> Voy a equivocarme a propósito. Si escribo mal la dirección, la imagen no carga, pero mira: aparece el texto alternativo. Por eso nunca lo dejes vacío. Lo corrijo y la imagen vuelve. Y un consejo: usa solo imágenes que sean tuyas o que tengan permiso para usarse, y no publiques fotos de otras personas sin su permiso.
>
> **(6:15 - 7:15) Enlaces**  
> Y llegamos a los enlaces, que son los que convierten un conjunto de páginas en un sitio web. Se escriben con la etiqueta a. El atributo `href` dice adónde lleva, y el texto de en medio es lo que se ve y lo que se toca. Enseguida lo probamos.
>
> **(7:15 - 8:00) Enlaces en una pestaña nueva**  
> Si quieres que el enlace abra en una pestaña nueva, agrega `target` igual a guion bajo blank. Y suma `rel` igual a noopener, que es una buena costumbre de seguridad cuando abres una pestaña nueva. Hago clic: MDN se abre en otra pestaña y mi página sigue aquí. Así tu visitante no pierde tu página.
>
> **(8:00 - 8:40) Antes de publicar**  
> Un aviso importante antes de seguir. Las páginas que haces en un editor en línea pueden verse en internet. Nunca escribas en ellas tu dirección, tu teléfono, tu apellido ni el nombre de tu colegio. Usa un apodo y comparte solo lo que te sentirías cómodo de que vea cualquier persona.
>
> **(8:40 - 9:30) Pausa y prueba**  
> Es tu turno. Pausa el video y agrega a tu página una lista con viñetas, una lista numerada y un enlace a tu sitio favorito. Si quieres usar una imagen, recuerda escribir su texto alternativo. Cuando termines, sigue con el video.
>
> **(9:30 - 10:00) Resumen**  
> Hoy aprendiste a crear listas con viñetas y numeradas, a poner imágenes con su texto alternativo y a crear enlaces. En la próxima lección empezamos con CSS, para darle color y estilo a tu página.

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 14:** Lámina de título. Texto en pantalla: «Lección 3 · Listas, imágenes y enlaces»
- **Listas con viñetas (0:30), Editor (JSFiddle), sin lámina:** JSFiddle con el fiddle de inicio (título, subtítulo y dos párrafos). El párrafo de pasatiempos se reemplaza por un `<ul>` con tres `<li>`: Dibujar, Jugar fútbol, Escuchar música. Se pulsa Ejecutar. Texto en pantalla: «`ul` = lista con viñetas» · «`li` = cada elemento de la lista». Anotación: llave sobre `ul` que abarca los `li`.
- **Listas numeradas (2:00), Editor (JSFiddle), sin lámina:** Debajo de la primera lista se escriben `<h2>Mis 3 metas del año</h2>` y un `<ol>` con tres metas, y se pulsa Ejecutar. Se sube la última meta al primer lugar, se pulsa Ejecutar (los números se ajustan) y se deshace con `Ctrl + Z`. Texto en pantalla: «`ol` = lista numerada». «¿Importa el orden? Usa `ol`.»
- **¿Viñetas o números? (3:00), Lámina 15:** Lámina con dos columnas: «Ingredientes» (`ul`, lista no ordenada) y «Pasos» (`ol`, lista ordenada). Texto en pantalla: «`<ul>`: lista no ordenada» · «`<ol>`: lista ordenada».
- **Imágenes (3:30), Lámina 16 (unos 5 s) y luego el editor (JSFiddle):** Primero la Lám. 16, con las etiquetas `img` y `a` que se verán en la lección. Luego, debajo del `h1`, se escribe `<img src="…/avatar.png" alt="Dibujo de Alex sonriendo con audífonos" width="200">` (con la dirección completa) y se pulsa Ejecutar. Aparece la imagen. Texto en pantalla: «`img` no necesita cierre» · «`src` = dónde está la imagen» · «`alt` = descripción». Anotación: subrayar `src` y `alt`.
- **Cuando la imagen no carga (5:00), Editor (JSFiddle), sin lámina:** En el `src` se borra una letra: `avatr.png`. Se pulsa Ejecutar: la imagen no carga y aparece el texto `alt`. Luego se corrige y se pulsa Ejecutar. Texto en pantalla: «Si la imagen no carga, aparece el `alt`». Anotación: círculo sobre el texto alternativo.
- **Enlaces (6:15), Editor (JSFiddle), sin lámina:** Al final se escribe el párrafo `<p>Mi sitio favorito para aprender:` con `<a href="https://developer.mozilla.org/es/">MDN Web Docs</a>` adentro, y se pulsa Ejecutar. Todavía no se hace clic. Texto en pantalla: «`a` = enlace» · «`href` = adónde lleva». Anotación: flecha de `href` al texto del enlace.
- **Enlaces en una pestaña nueva (7:15), Editor (JSFiddle), sin lámina:** Dentro de la etiqueta `a`, después del `href`, se agrega `target="_blank" rel="noopener"` y se pulsa Ejecutar. Al hacer clic, MDN se abre en una pestaña nueva; se cierra y se vuelve a JSFiddle. Texto en pantalla: «`target="_blank"` = pestaña nueva» · «`rel="noopener"` = buena costumbre de seguridad».
- **Antes de publicar (8:00), Lámina 17:** Lámina «Antes de publicar», con una tarjeta de perfil y un ojo tachado: nunca publicar la dirección, el teléfono, el apellido ni el colegio. Texto en pantalla: «Antes de publicar: ¿es información privada?» «Usa un apodo».
- **Pausa y prueba (8:40), Lámina 18:** Tarjeta de pausa de 5 segundos con cuenta regresiva. Texto en pantalla: «Pausa y prueba» · «Tómate el tiempo que necesites» · «Agrega una lista con tus pasatiempos» · «Agrega una lista numerada con tus metas» · «Agrega un enlace a tu sitio favorito».
- **Resumen (9:30), Lámina 19:** Lámina de resumen. Texto en pantalla: «Listas: no ordenadas (`ul`) y ordenadas (`ol`)» · «Imágenes: la etiqueta `img`, con `src` y `alt`» · «Enlaces: la etiqueta `a`, con `href` y `target`».

## 4. Pregunta para pensar

¿por qué es mejor escribir «Dibujo de Alex sonriendo con audífonos» que dejar el `alt` vacío o poner «imagen»?
