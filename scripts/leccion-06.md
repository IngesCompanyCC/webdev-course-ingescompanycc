# Lección 6: Errores comunes y próximos pasos

_(Contenido para los instructores)_

**Objetivo:** Al terminar, el estudiante puede reconocer los errores más comunes al escribir HTML y CSS, encontrarlos con ayuda del editor y de un validador en línea, y sabe cómo seguir aprendiendo.

**Palabras nuevas:** error, validar, validador, depurar (encontrar y corregir errores).

## 1. Estructura de carpetas (GitHub)

```text
/starter-files/leccion-06        # Código de inicio de la lección
├── index.html
└── styles.css

/completed-examples/leccion-06   # Código completo de la lección
├── index.html
└── styles.css
```

## 2. Guion del video (9 minutos)

> Los tiempos son los del audio (unos 8:01). Con las tarjetas de pausa, los Ejecutar y las transiciones de la edición, el video llega a unos 9 minutos. El guion detallado para grabar está en `grabacion/leccion-06.md` (solo para el equipo).

> **(0:00 - 0:35) Introducción**  
> ¡Hola! Te doy la bienvenida a la última lección del curso. Ya sabes crear una página. Hoy vas a aprender algo que hace cualquier persona que programa, incluso con años de experiencia: encontrar y corregir errores. Equivocarse es normal: hasta los videojuegos más famosos salen con errores, que luego se arreglan con actualizaciones. Lo importante es saber cómo buscarlos. ¡Hoy te conviertes en detective de código!
>
> **(0:35 - 1:08) Los 5 errores más comunes**  
> Estos son cinco errores muy comunes. Una etiqueta que se abre y nunca se cierra. Una imagen sin texto alternativo. Una clase en CSS escrita sin el punto delante. Una propiedad con una letra de más o de menos. Y un punto y coma que se olvidó. Les pasan a todos, así que vale la pena reconocerlos a primera vista.
>
> **(1:08 - 1:49) Dos tipos de errores**  
> Estos errores son de dos tipos. Los errores en el HTML cambian la estructura de la página: por ejemplo, una etiqueta sin cerrar hace que lo que viene después quede dentro de ella. Los errores en el CSS no cambian el contenido: el navegador ignora la regla que no entiende, sin ningún aviso, y ese estilo no se aplica. Por eso, cuando algo se ve raro, pregúntate primero: ¿falla la estructura o falla el estilo?
>
> **(1:49 - 2:25) El reto: encuentra los 5 errores**  
> Te presento una página de perfil con cinco errores escondidos, uno de cada tipo. Fíjate en el resultado: ¿qué se ve raro? Ahora te reto: pausa el video, abre el enlace de la descripción y trata de encontrar los cinco. Ten paciencia: es un juego de detectives. Cuando termines, sigue con el video.
>
> **(2:25 - 3:06) Una etiqueta sin cerrar**  
> Vamos por el primero. Mira la lista de pasatiempos: se ve grande y en negrita, como un título. Eso suele pasar cuando una etiqueta no se cerró. En el código, el h2 de Mis pasatiempos no tiene su etiqueta de cierre, así que todo lo que viene después, hasta el final de esa sección, quedó dentro del título. Lo cierro con barra h2 y pulso Ejecutar. ¡La lista volvió a la normalidad!
>
> **(3:06 - 3:39) Una clase sin el punto**  
> Segundo caso: la tarjeta perdió el borde y no está centrada. En el CSS, la regla se llama perfil, sin punto. Sin el punto, CSS busca una etiqueta llamada perfil, que no existe. Le agrego el punto, pulso Ejecutar… ¡y vuelve la tarjeta, con su borde y centrada! Recuerda: en CSS, el punto significa busca esta clase.
>
> **(3:39 - 4:15) Una propiedad mal escrita**  
> Tercer caso: el fondo azul no aparece. Reviso el body y veo backgroud-color: le falta una letra n. El navegador no avisa nada: simplemente ignora lo que no entiende. Es como la contraseña del wifi: con una letra de menos, no funciona. Agrego la n, pulso Ejecutar y aparece el fondo. Cuando algo no cambia, revisa letra por letra cómo escribiste el nombre.
>
> **(4:15 - 4:46) Un punto y coma olvidado**  
> Cuarto caso: los subtítulos no tienen el color verde. En la regla de h2, a la línea del color le falta el punto y coma. Sin él, el navegador junta esa línea con la siguiente y no entiende ninguna de las dos. Lo agrego, pulso Ejecutar… ¡y recuperan su color y su tamaño!
>
> **(4:46 - 5:28) Una imagen sin alt**  
> Y el último error no se ve a simple vista: la imagen de la mascota no tiene texto alternativo. Por eso es bueno revisar el código, además de mirar la pantalla. Agrego alt con la descripción: Dibujo de Miso, un gato naranja. Ejecutar: la página se ve igual, pero ahora está corregida. Como ya encontré los cinco errores, borro el comentario del reto.
>
> **(5:28 - 6:18) El validador**  
> Hay una herramienta que te ayuda a encontrar errores: un validador. Es una página gratuita donde pegas tu código y te avisa lo que está mal, con el número de línea. Pego la página con errores y pulso Check. Aquí encontró la etiqueta sin cerrar y la imagen sin texto alternativo. Úsalo cuando tu página no se vea como esperas. También hay un validador de CSS, pero ningún validador encuentra todo; por ejemplo, la clase sin punto no la marca. Por eso, revisa también con tus propios ojos.
>
> **(6:18 - 6:58) Buenas prácticas**  
> Para cometer menos errores, sigue cuatro buenas prácticas. Primero, aplica sangría: cada elemento que va dentro de otro se escribe un poco más adentro, así ves dónde abre y dónde cierra. Segundo, usa nombres de clase que digan para qué sirven, como destacado. Tercero, revisa el resultado después de cada cambio, y no solo al final. Y cuarto, pasa tu código por el validador antes de compartir tu página.
>
> **(6:58 - 7:38) ¿Y ahora qué?**  
> ¿Y ahora qué? Primero, explora la documentación web de MDN: es gratuita, está en español y es una de las mejores fuentes. Segundo, haz otra página sobre algo que te guste: tu club, tu banda favorita o una receta. Tercero, cuando tengas varias páginas, únelas con enlaces: así tendrás tu propio sitio web. Y cuarto, practica un poco cada día: es mejor veinte minutos diarios que cuatro horas de golpe.
>
> **(7:38 - 8:01) Cierre**  
> ¡Lo lograste! Terminaste el curso. Al empezar no sabías cómo se hace una página web, y ahora has creado la tuya. Comparte lo que hiciste con tu familia y tus amistades. Gracias por acompañarnos. ¡Sigue creando!

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 32:** Lámina de título. Sin texto añadido en pantalla.
- **Los 5 errores más comunes (0:35), Lámina 33:** Lámina con la lista de los 5 errores comunes; al editar se resaltan de uno en uno. Sin texto añadido en pantalla.
- **Dos tipos de errores (1:08), Lámina 34:** Lámina de dos columnas: errores en el HTML y errores en el CSS. Sin texto añadido en pantalla.
- **El reto: encuentra los 5 errores (1:49), Editor (el fiddle con errores) y, al final, Lámina 35:** JSFiddle con la página con errores; no se escribe nada. Se hace un recorrido por el resultado. Después, la Lámina 35: tarjeta de pausa de unos 5 segundos. Texto en pantalla (solo durante el editor): «Esta página tiene 5 errores». Anotación: signos de interrogación sobre lo que se ve raro.
- **Una etiqueta sin cerrar (2:25), Editor (JSFiddle), sin lámina:** Se vuelve al fiddle. Se pasa el cursor por la lista de pasatiempos, que se ve en negrita. Se revisa el código del `h2`, se agrega `</h2>` y se pulsa Ejecutar. Texto en pantalla: «Error 1: falta `</h2>`». Anotación: círculo sobre el `<h2>` sin cierre.
- **Una clase sin el punto (3:06), Editor (JSFiddle), sin lámina:** Se compara el resultado con el CSS: la tarjeta no tiene borde ni está centrada. Se busca la regla `perfil`, se le agrega el punto (`.perfil`) y se pulsa Ejecutar. Texto en pantalla: «Error 3: falta el punto» · «Clase = `.nombre`».
- **Una propiedad mal escrita (3:39), Editor (JSFiddle), sin lámina:** El fondo no es azul. Se revisa el `body`, se corrige `backgroud-color` por `background-color` y se pulsa Ejecutar. Texto en pantalla: «Error 4: `backgroud` ≠ `background`». Anotación: subrayar el lugar donde falta la n.
- **Un punto y coma olvidado (4:15), Editor (JSFiddle), sin lámina:** Los subtítulos no son verdes. Se revisa la regla de `h2`, se agrega el `;` al final de `color: #0f766e` y se pulsa Ejecutar. Texto en pantalla: «Error 5: falta el `;`».
- **Una imagen sin alt (4:46), Editor (JSFiddle), sin lámina:** Se revisa la imagen de la mascota. Se agrega `alt="Dibujo de Miso, un gato naranja"` y se pulsa Ejecutar: no se ve ningún cambio. Al final se borra el comentario del reto («Esta página tiene 5 errores…»). Texto en pantalla: «Error 2: falta `alt`».
- **El validador (5:28), navegador con el validador, sin lámina:** Se abre el validador del W3C. Se pega el documento completo con errores, se pulsa «Check» y se muestran los avisos de la etiqueta sin cerrar y de la imagen sin `alt`. Texto en pantalla, en una franja abajo y antes de que aparezcan los avisos: «Un validador revisa tu código por ti». Anotación: recuadros naranjas sobre el aviso del `h2` sin cerrar y el del `alt`, con su número de línea.
- **Buenas prácticas (6:18), Lámina 36:** Lámina con cuatro buenas prácticas, cada una con su ícono. Sin texto añadido en pantalla.
- **¿Y ahora qué? (6:58), Lámina 37:** Lámina de próximos pasos con cuatro ideas. Sin texto añadido en pantalla.
- **Cierre (7:38), Lámina 38:** Lámina final con un mensaje de cierre. Sin texto añadido en pantalla.

## 4. Pregunta para pensar

Si una regla de CSS no se aplica y el navegador no muestra ningún aviso, ¿qué tres cosas revisarías primero?
