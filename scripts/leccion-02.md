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

> **(0:00 - 0:40) Introducción**  
> En la lección anterior viste que HTML define el contenido y la estructura de una página. Hoy vas a escribir la tuya. Al terminar sabrás qué son las etiquetas, los elementos y los atributos, y tendrás tu primer título y tus primeros párrafos.
>
> **(0:40 - 2:00) Etiqueta, contenido y elemento**  
> Todo en HTML se escribe con etiquetas. Una etiqueta es una palabra entre los signos menor que y mayor que. Casi siempre van en pareja: una abre y otra cierra, y la de cierre lleva una barra. Lo que queda en medio es el contenido. Las tres cosas juntas forman un elemento. La etiqueta indica qué tipo de contenido es: un título, un párrafo, una lista.
>
> **(2:00 - 3:30) Así se ve una página completa**  
> Así es una página completa. La primera línea le dice al navegador que es HTML moderno. Luego viene `html`, y adentro dos partes. El `head` es la información sobre la página: por ejemplo, el título que aparece en la pestaña del navegador y la línea que permite ver bien las tildes y la eñe. El `body` es lo que se ve: títulos, textos, imágenes. Fíjate también en `lang="es"`: es un atributo que dice que la página está en español. Más adelante veremos qué son los atributos.
>
> **(3:30 - 3:50) El panel HTML de JSFiddle**  
> Ahora vamos a escribir. En JSFiddle no hace falta la parte de arriba, porque el editor ya la prepara por nosotros. Por eso, en el panel HTML escribimos solo lo que iría dentro del `body`.
>
> **(3:50 - 4:40) El título principal**  
> Empecemos con un título. Escribo menor que, h1, mayor que; el texto; y cierro con menor que, barra, h1, mayor que. Pulso Ejecutar y mira el resultado: apareció mi título, grande y en negrita. Usa un apodo o un nombre inventado, no tu apellido ni datos privados.
>
> **(4:40 - 5:40) Párrafos**  
> Ahora un párrafo, con la etiqueta p. Una pista importante: si presionas Enter dentro del párrafo, la página no cambia de línea. HTML ignora esos saltos. Para separar el texto se usa un párrafo nuevo, con su propia etiqueta de apertura y de cierre.
>
> **(5:40 - 7:00) Títulos del h1 al h6**  
> Los títulos van del h1 al h6, como los títulos de un libro. El h1 es el título principal y conviene usar uno solo por página. El h2 es un subtítulo, el h3 es un subtítulo del h2, y así sigue. No los elijas por el tamaño: elígelos por la importancia. El tamaño lo cambiaremos con CSS.
>
> **(7:00 - 7:50) Atributos**  
> Ahora, los atributos. Un atributo es información extra que se escribe dentro de la etiqueta de apertura, con un nombre, un signo igual y un valor entre comillas. Agrego `title` y mi mensaje. Si paso el cursor sobre el título, aparece. En las próximas lecciones usaremos atributos para imágenes y enlaces.
>
> **(7:50 - 8:30) Comentarios**  
> Una última herramienta: los comentarios. Es una nota para ti o para tu equipo que el navegador no muestra. Se escribe entre menor que, signo de exclamación y dos guiones, y se cierra con dos guiones y mayor que. Úsalos para ordenar tu código.
>
> **(8:30 - 9:20) Pausa y prueba**  
> Tu turno. Pausa el video y crea tu página: un título con tu apodo, un párrafo sobre ti, un subtítulo y otro párrafo. Si algo no sale, revisa que cada etiqueta que abriste también esté cerrada. Cuando termines, continúa con el video.
>
> **(9:20 - 10:00) Resumen**  
> Hoy aprendiste a escribir HTML: las etiquetas y los elementos, los atributos, los títulos, los párrafos y los comentarios. En la próxima lección agregaremos listas, imágenes y enlaces para que tu página tenga más contenido.

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 7:** Lámina de título. Texto en pantalla: «Lección 2 · Tu primera página HTML»
- **Etiqueta, contenido y elemento (0:40), Lámina 8:** Lámina con `<p>Hola</p>` en grande. Cada parte ya está en su color (apertura, contenido y cierre) dentro del marco «Elemento». Texto en pantalla: «Etiqueta de apertura» · «Contenido» · «Etiqueta de cierre». Anotación: llave que agrupa todo y dice «Elemento».
- **Así se ve una página completa (2:00), Lámina 9:** Lámina con el esqueleto completo de una página (`<!DOCTYPE html>`, `<html lang="es">`, `<head>` con `<meta charset="UTF-8">` y `<title>`, y `<body>`). A la derecha se explica qué es `head` y qué es `body`. Texto en pantalla: «`head`: información de la página» · «`body`: lo que se ve». Anotación: flecha del `<title>` a una pestaña del navegador.
- **El panel HTML de JSFiddle (3:30), Editor (JSFiddle), sin lámina:** JSFiddle con el fiddle de inicio: los paneles HTML y CSS vacíos. Se señala el panel HTML; no se escribe nada. Texto en pantalla: «En JSFiddle solo escribimos lo de `body`».
- **El título principal (3:50), Editor (JSFiddle), sin lámina:** En la primera línea del panel HTML se escribe despacio `<h1>Hola, soy Alex</h1>` y se pulsa Ejecutar. El resultado muestra el título grande. Texto en pantalla: «`h1` = título principal». Zoom al panel mientras se escribe.
- **Párrafos (4:40), Editor (JSFiddle), sin lámina:** Debajo del `h1` se escribe `<p>Estoy en secundaria y me encanta aprender cosas nuevas.</p>` y se pulsa Ejecutar. Luego se presiona `Enter` dentro del párrafo, después de «secundaria», se pulsa Ejecutar y se muestra que el texto sigue en la misma línea. Se deshace con `Ctrl + Z`. Texto en pantalla: «`p` = párrafo». Anotación: señalar que `Enter` no cambia de línea en la página.
- **Títulos del h1 al h6 (5:40), Editor y, al final, Lámina 10 (unos 8 s):** Debajo del párrafo se agregan `<h2>Mis pasatiempos</h2>` y `<p>Me gusta dibujar, jugar fútbol y escuchar música.</p>`, y se pulsa Ejecutar. Se cambia el `h2` por `h3` y luego por `h4` (en la apertura y en el cierre), pulsando Ejecutar cada vez, y se vuelve a `h2`. Al final, la Lám. 10: el índice de un libro con h1, h2, h3 y h4. Texto en pantalla: «`h1` a `h6`: del más importante al menos importante». «Un solo `h1` por página».
- **Atributos (7:00), Lámina 11 (unos 5 s) y luego el editor (JSFiddle):** Después de la Lám. 11, en el editor se agrega el atributo `title` al `h1`: `<h1 title="¡Pasaste el cursor por aquí!">` y se pulsa Ejecutar. Se pasa el cursor sobre el título en Resultado y aparece el texto emergente. Texto en pantalla: «Atributo = `nombre="valor"`». Anotación: subrayar `title` y su valor.
- **Comentarios (7:50), Editor (JSFiddle), sin lámina:** Arriba del `h2` se escribe el comentario `<!-- Aquí empiezan mis pasatiempos -->` y se pulsa Ejecutar. No aparece en el resultado. Texto en pantalla: «Comentario: una nota que el navegador no muestra».
- **Pausa y prueba (8:30), Lámina 12:** Tarjeta de pausa de 5 segundos con cuenta regresiva. Texto en pantalla: «Pausa y prueba» · «Tómate el tiempo que necesites» · «Escribe un título con tu apodo» · «Agrega un párrafo sobre ti» · «Agrega un subtítulo y otro párrafo».
- **Resumen (9:20), Lámina 13:** Lámina de resumen con cuatro puntos. Texto en pantalla: «Elementos: etiqueta de apertura, contenido y cierre» · «Atributos: se escriben como `nombre="valor"`» · «Títulos: del `h1` al `h6`, según su importancia» · «Párrafos: bloques de texto con la etiqueta `p`».

## 4. Pregunta para pensar

¿qué pasa en la página si abres un `<p>` y olvidas cerrarlo? (Se contesta en la lección 6.)
