# Lección 2: Tu primera página HTML

_(Contenido para los instructores)_

**Objetivo:** Al terminar, el estudiante puede explicar qué son una etiqueta, un elemento y un atributo, y escribir en un editor en línea una página con un título, un subtítulo y párrafos.

**Palabras nuevas:** etiqueta, elemento, atributo, contenido, encabezado, párrafo, comentario.

## 1. Estructura de carpetas (GitHub)

```text
/starter-files/leccion-02        # Código de inicio de la lección
└── index.html

/completed-examples/leccion-02   # Código completo de la lección
└── index.html
```

## 2. Guion del video (10 minutos)

> Los tiempos son los del audio (unos 8:48). Con las tarjetas de pausa, los Ejecutar y las transiciones de la edición, el video llega a unos 10 minutos. El guion detallado para grabar está en `grabacion/leccion-02.md` (solo para el equipo).

> **(0:00 - 0:40) Introducción**  
> ¡Hola! Te doy la bienvenida a la lección 2. En la lección anterior viste que HTML define el contenido y la estructura de una página. Hoy vas a escribir la tuya, desde cero. Al terminar sabrás qué son las etiquetas, los elementos y los atributos, y tendrás tu primer título y tus primeros párrafos. Es como aprender las piezas de un juego de construcción: con pocas piezas ya puedes armar mucho. ¡Vamos!
>
> **(0:40 - 1:36) Etiqueta, contenido y elemento**  
> Todo en HTML se escribe con etiquetas. Una etiqueta es una palabra entre los signos menor que y mayor que, como esta: p, de párrafo. Casi siempre van en pareja: una abre y otra cierra, y la de cierre lleva una barra. Lo que queda en medio es el contenido; aquí, la palabra Hola. Las tres cosas juntas, apertura, contenido y cierre, forman un elemento. La etiqueta le dice al navegador qué tipo de contenido es: un título, un párrafo, una lista. Es como las etiquetas de las cajas en una mudanza: cocina, libros, ropa. Sabes qué hay adentro sin abrirlas.
>
> **(1:36 - 2:32) Así se ve una página completa**  
> Así es una página completa. La primera línea, DOCTYPE html, le dice al navegador que es HTML moderno. Luego viene la etiqueta html, y adentro hay dos partes. El head es la información sobre la página: por ejemplo, el título que aparece en la pestaña del navegador, y la línea meta charset, que permite ver bien las tildes y la eñe. El body es lo que se ve: títulos, textos, imágenes. Fíjate también en lang igual a es: es un atributo que dice que la página está en español. En esta misma lección vas a ver qué son los atributos.
>
> **(2:32 - 3:08) El panel HTML de JSFiddle**  
> Ahora vamos a escribir. En JSFiddle no hace falta la parte de arriba, porque el editor ya la prepara por nosotros. Por eso, en el panel HTML escribimos solo lo que iría dentro del body. JSFiddle arma por ti el DOCTYPE, el head y el body, y así tú te concentras en lo que se ve. Aquí está el panel, vacío y listo para ti.
>
> **(3:08 - 3:57) El título principal**  
> ¡Escribe conmigo! Empecemos con un título. Escribo menor que, h1, mayor que; el texto, Hola, soy Alex; y cierro con menor que, barra, h1, mayor que. Pulso Ejecutar y… ¡mira! Apareció mi título, grande y en negrita. h1 viene de heading 1, encabezado número uno. Y fíjate en la barra del cierre: si la olvidas, el navegador no sabe dónde termina el título. En la lección 6 vas a ver qué pasa en ese caso.
>
> **(3:57 - 4:54) Párrafos**  
> Ahora un párrafo, con la etiqueta p. Debajo del título escribo: Estoy en secundaria y me encanta aprender cosas nuevas. Ejecutar. Una pista importante: si presiono Enter dentro del párrafo, después de la palabra secundaria, y pulso Ejecutar… la página no cambia de línea. HTML ignora esos saltos. Y lo mismo pasa con los espacios: si escribes diez espacios seguidos, el navegador muestra solo uno. Deshago el salto con Control Z. Para separar el texto se usa un párrafo nuevo, con su propia etiqueta de apertura y de cierre.
>
> **(4:54 - 6:01) Títulos del h1 al h6**  
> Debajo agrego un subtítulo con h2, Mis pasatiempos, y otro párrafo: Me gusta dibujar, jugar fútbol y escuchar música. Ejecutar. Los títulos van del h1 al h6. Prueba rápida: cambio h2 por h3, en la apertura y en el cierre, y pulso Ejecutar: el subtítulo se achica. Con h4, más pequeño todavía. Lo regreso a h2. Funcionan como el índice de un libro: el h1 es el título del libro, y conviene usar uno solo por página; el h2 es un capítulo; el h3, una sección del capítulo, y así sigue. No los elijas por el tamaño: elígelos por su importancia. El tamaño lo cambiaremos con CSS.
>
> **(6:01 - 7:01) Atributos**  
> Ahora, los atributos. Un atributo es información extra que se escribe dentro de la etiqueta de apertura: un nombre, un signo igual y un valor entre comillas. Vamos a probarlo. En el h1, después de h1 y antes del mayor que, escribo title, igual, y entre comillas: ¡Pasaste el cursor por aquí! Ejecutar. Paso el cursor sobre el título y… ¡aparece mi mensaje! Los atributos son como las opciones de un personaje en un videojuego: el personaje es el mismo, pero le cambias detalles. En la próxima lección usaremos atributos para poner imágenes y enlaces.
>
> **(7:01 - 7:49) Comentarios**  
> Una última herramienta: los comentarios. Son notas para ti o para tu equipo que el navegador no muestra. Se escriben entre menor que, signo de exclamación y dos guiones, y se cierran con dos guiones y mayor que. Arriba del h2 escribo: Aquí empiezan mis pasatiempos. Ejecutar. No aparece en la página, y así debe ser. Úsalos para ordenar tu código, por ejemplo, para recordar dónde empieza cada parte cuando tu página crezca.
>
> **(7:49 - 8:17) Pausa y prueba**  
> ¡Te toca! Pausa el video y crea tu propia página en el enlace de la descripción. Escribe tu propio título, agrega un párrafo sobre ti, un subtítulo y otro párrafo. Si algo no sale, revisa que cada etiqueta que abriste también esté cerrada. Cuando termines, sigue con el video.
>
> **(8:17 - 8:48) Resumen**  
> ¡Muy bien! Hoy escribiste tu primera página en HTML. Aprendiste qué son los elementos, con su etiqueta de apertura, su contenido y su cierre; los atributos; los títulos del h1 al h6, y los párrafos. En la próxima lección vas a agregar listas, imágenes y enlaces, para que tu página tenga mucho más contenido. ¡Nos vemos ahí!

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 7:** Lámina de título. Sin texto añadido en pantalla.
- **Etiqueta, contenido y elemento (0:40), Lámina 8:** Lámina con `<p>Hola</p>` en grande; cada parte en su color (apertura, contenido y cierre) dentro del marco «Elemento», y se resalta en el orden de la narración. Sin texto añadido en pantalla. Anotación: resaltar el marco «Elemento».
- **Así se ve una página completa (1:36), Lámina 9:** Lámina con el esqueleto completo de una página (`<!DOCTYPE html>`, `<html lang="es">`, `<head>` con `<meta charset="UTF-8">` y `<title>`, y `<body>`). Sin texto añadido en pantalla. Anotación: resaltar `<title>` y la frase «El título aparece en la pestaña».
- **El panel HTML de JSFiddle (2:32), Editor (JSFiddle), sin lámina:** JSFiddle con el fiddle de inicio: los paneles HTML y CSS vacíos. Se señala el panel HTML; no se escribe nada. Texto en pantalla: «En JSFiddle solo escribimos lo de `body`» · «JSFiddle arma el resto por ti».
- **El título principal (3:08), Editor (JSFiddle), sin lámina:** En la primera línea del panel HTML se escribe despacio `<h1>Hola, soy Alex</h1>` y se pulsa Ejecutar: el resultado muestra el título grande. Texto en pantalla: «`h1` = título principal (heading 1)» · «El cierre lleva barra: `</h1>`». Zoom al panel mientras se escribe.
- **Párrafos (3:57), Editor (JSFiddle), sin lámina:** Debajo del `h1` se escribe `<p>Estoy en secundaria y me encanta aprender cosas nuevas.</p>` y se pulsa Ejecutar. Luego se presiona `Enter` dentro del párrafo, se pulsa Ejecutar y el texto sigue en la misma línea; se deshace con `Ctrl + Z`. Texto en pantalla: «`p` = párrafo» · «Los saltos de línea y los espacios de más no se ven». Anotación: señalar que `Enter` no cambia de línea en la página.
- **Títulos del h1 al h6 (4:54), Editor y, al final, Lámina 10 (unos 8 s):** Debajo del párrafo se agregan `<h2>Mis pasatiempos</h2>` y `<p>Me gusta dibujar, jugar fútbol y escuchar música.</p>`, y se pulsa Ejecutar. Prueba rápida: `h3`, `h4` y vuelta a `h2`, con Ejecutar cada vez. Al final, la Lámina 10: el índice de un libro con h1, h2, h3 y h4. Texto en pantalla (solo durante el editor): «`h1` a `h6`: del más importante al menos importante».
- **Atributos (6:01), Lámina 11 (unos 5 s) y luego el editor (JSFiddle):** Primero la Lámina 11. Luego, en el editor, se agrega el atributo `title` al `h1`: `<h1 title="¡Pasaste el cursor por aquí!">` y se pulsa Ejecutar; al pasar el cursor sobre el título aparece el texto emergente. Texto en pantalla (solo durante el editor): «Pasa el cursor sobre el título». Anotación: subrayar `title` y su valor.
- **Comentarios (7:01), Editor (JSFiddle), sin lámina:** Arriba del `h2` se escribe el comentario `<!-- Aquí empiezan mis pasatiempos -->` y se pulsa Ejecutar: no aparece en el resultado. Texto en pantalla: «Comentario: una nota que el navegador no muestra».
- **Pausa y prueba (7:49), Lámina 12:** Tarjeta de pausa de 5 segundos. Sin texto añadido en pantalla.
- **Resumen (8:17), Lámina 13:** Lámina de resumen con cuatro tarjetas. Sin texto añadido en pantalla.

## 4. Pregunta para pensar

¿qué pasa en la página si abres un `<p>` y olvidas cerrarlo? (Se contesta en la lección 6.)
