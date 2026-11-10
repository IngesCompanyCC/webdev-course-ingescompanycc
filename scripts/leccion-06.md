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

> **(0:00 - 0:45) Introducción**  
> Ya sabes crear una página. En esta última lección vas a aprender algo que hace cualquier persona que programa, incluso con años de experiencia: encontrar y corregir errores. Equivocarse es normal; lo importante es saber cómo buscarlos.
>
> **(0:45 - 1:45) Los 5 errores más comunes**  
> Estos son cinco errores muy comunes. Una etiqueta que se abre y nunca se cierra. Una imagen sin texto alternativo. Una clase en CSS escrita sin el punto delante. Una propiedad con una letra de más o de menos. Y un punto y coma que se olvidó. Los cinco le pasan a todo el mundo.
>
> **(1:45 - 2:30) Dos tipos de errores**  
> Estos errores son de dos tipos. Los errores en el HTML cambian la estructura de la página: por ejemplo, una etiqueta sin cerrar hace que lo que viene después quede dentro de ella. Los errores en el CSS no cambian el contenido: el navegador ignora la regla que no entiende, sin mostrar ningún aviso, y ese estilo no se aplica. Por eso, cuando algo se ve raro, pregúntate primero: ¿falla la estructura o falla el estilo?
>
> **(2:30 - 2:55) El reto: encuentra los 5 errores**  
> Te presento una página de perfil con cinco errores escondidos, uno de cada tipo. Fíjate en el resultado: ¿qué se ve raro? Ahora te reto: pausa el video, abre el fiddle de la descripción y trata de encontrar los cinco. Ten paciencia; es un juego de detectives. Cuando termines, sigue con el video.
>
> **(2:55 - 3:30) Una etiqueta sin cerrar**  
> Vamos por el primero. Mira la lista de pasatiempos: se ve grande y en negrita, como un título. Eso suele pasar cuando una etiqueta no se cerró. Si miro el código, encuentro que el `h2` de «Mis pasatiempos» no tiene su etiqueta de cierre. Todo lo que viene después, hasta el final de esa sección, queda adentro del título. Lo cierro y todo vuelve a la normalidad.
>
> **(3:30 - 4:15) Una clase sin el punto**  
> Segundo caso: la tarjeta perdió el borde y no está centrada. En el CSS, la regla se llama `perfil` sin punto. Sin el punto, CSS busca una etiqueta llamada perfil, que no existe. Le agrego el punto y listo.
>
> **(4:15 - 5:00) Una propiedad mal escrita**  
> Tercer caso: el fondo azul no aparece. Reviso el body y veo `backgroud-color`: le falta una letra n. El navegador no marca ningún aviso: simplemente ignora lo que no entiende. Por eso, cuando algo no cambia, revisa cómo escribiste el nombre.
>
> **(5:00 - 5:45) Un punto y coma olvidado**  
> Cuarto caso: los subtítulos no tienen el color verde. En la regla de h2, a la línea del color le falta el punto y coma. Sin él, el navegador junta esa línea con la siguiente y no entiende ninguna de las dos. Lo agrego y recuperan su color y su tamaño.
>
> **(5:45 - 6:15) Una imagen sin alt**  
> Y el último error no se ve a simple vista: la imagen de la mascota no tiene texto alternativo. Por eso es bueno revisar el código además de mirar la pantalla. Lo agrego y la página queda corregida. Como ya encontré los cinco errores, borro el comentario del reto.
>
> **(6:15 - 7:00) El validador**  
> Hay una herramienta que te ayuda a encontrar errores: un validador. Es una página gratuita donde pegas tu código y te avisa lo que está mal, con el número de línea. Aquí encontró la etiqueta sin cerrar y la imagen sin texto alternativo. Úsalo cuando tu página no se vea como esperas.
>
> **(7:00 - 7:45) Buenas prácticas**  
> Para cometer menos errores, sigue cuatro buenas prácticas. Primero, aplica sangría: cada elemento que va dentro de otro se escribe un nivel más adentro, así ves dónde abre y dónde cierra. Segundo, usa nombres de clase que digan para qué sirven, como destacado. Tercero, revisa el resultado después de cada cambio, y no solo al final. Y cuarto, pasa tu código por el validador antes de compartir tu página.
>
> **(7:45 - 8:45) ¿Y ahora qué?**  
> ¿Y ahora qué? Primero, explora la documentación web de MDN: es gratuita, está en español y es una de las mejores fuentes. Segundo, practica con una página sobre algo que te guste: tu club, tu banda favorita o una receta. Tercero, cuando tengas varias páginas, únelas con enlaces: así tendrás tu propio sitio web. Y cuarto, practica un poco cada día: es mejor veinte minutos diarios que cuatro horas un día.
>
> **(8:45 - 9:15) Cierre**  
> Terminaste el curso. Al empezar este curso no sabías cómo se hace una página web, y ahora has creado la tuya. Comparte lo que hiciste con tu familia y tus amistades, y recuerda no publicar datos privados. Gracias por acompañarnos, y sigue creando.

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 32:** Lámina de título. Texto en pantalla: «Lección 6 · Errores comunes y próximos pasos»
- **Los 5 errores más comunes (0:45), Lámina 33:** Lámina con la lista de los 5 errores comunes, en una sola lámina; al editar el video se pueden resaltar de uno en uno. Texto en pantalla: «1. Una etiqueta sin cerrar» · «2. Una imagen sin `alt`» · «3. Una clase sin el punto» · «4. Una propiedad mal escrita» · «5. Un punto y coma olvidado».
- **Dos tipos de errores (1:45), Lámina 34:** Lámina de dos columnas: errores en el HTML y errores en el CSS. Texto en pantalla: «En el HTML: una etiqueta sin cerrar cambia la estructura» · «En el CSS: una regla mal escrita se ignora sin aviso».
- **El reto: encuentra los 5 errores (2:30), Editor (el fiddle con errores) y, al final, Lámina 35:** JSFiddle con la página con errores; no se escribe nada. Se hace un recorrido por el resultado. Después, la Lám. 35: tarjeta de pausa de 5 segundos. Texto (sobre el editor): «Esta página tiene 5 errores». Lám. 35: «Encuentra los 5 errores» · «Tómate el tiempo que necesites» · «Abre el enlace de la descripción» · «Mira el resultado: ¿qué se ve raro?». Anotación: marcar con signos de interrogación lo que se ve raro.
- **Una etiqueta sin cerrar (2:55), Editor (JSFiddle), sin lámina:** Se vuelve al fiddle. Se pasa el cursor por la lista de pasatiempos, que se ve en negrita. Se revisa el código del `h2`, se agrega `</h2>` y se pulsa Ejecutar. Texto en pantalla: «Error 1: falta `</h2>`». Anotación: círculo sobre el `<h2>` sin cierre.
- **Una clase sin el punto (3:30), Editor (JSFiddle), sin lámina:** Se compara el resultado con el CSS: la tarjeta no tiene borde ni está centrada. Se busca la regla `perfil`, se le agrega el punto (`.perfil`) y se pulsa Ejecutar. Texto en pantalla: «Error 3: falta el punto». «Clase = `.nombre`».
- **Una propiedad mal escrita (4:15), Editor (JSFiddle), sin lámina:** El fondo no es azul. Se revisa el `body`, se corrige `backgroud-color` por `background-color` y se pulsa Ejecutar. Texto en pantalla: «Error 4: `backgroud` ≠ `background`». Anotación: subrayar el lugar donde falta la n.
- **Un punto y coma olvidado (5:00), Editor (JSFiddle), sin lámina:** Los subtítulos no son verdes. Se revisa la regla de `h2`, se agrega el `;` al final de `color: #0f766e` y se pulsa Ejecutar. Texto en pantalla: «Error 5: falta el `;`».
- **Una imagen sin alt (5:45), Editor (JSFiddle), sin lámina:** Se revisa la imagen de la mascota. Se agrega `alt="Dibujo de Miso, un gato naranja"` y se pulsa Ejecutar: no se ve ningún cambio. Al final se borra el comentario del reto («Esta página tiene 5 errores…»). Texto en pantalla: «Error 2: falta `alt`».
- **El validador (6:15), navegador con el validador, sin lámina:** Se abre el validador del W3C. Se pega el documento completo con errores, se pulsa «Check» y se muestran los avisos. Texto en pantalla: «Un validador revisa tu código por ti». Anotación: marcar un aviso con su número de línea.
- **Buenas prácticas (7:00), Lámina 36:** Lámina con cuatro buenas prácticas, cada una con su ícono. Texto en pantalla: «Sangría: aplica sangría a cada elemento anidado» · «Nombres claros: clases descriptivas, como `.destacado`» · «Prueba seguido: revisa el resultado tras cada cambio» · «Valida: revisa tu código con el validador».
- **¿Y ahora qué? (7:45), Lámina 37:** Lámina de próximos pasos con cuatro ideas. Texto en pantalla: «MDN: documentación web gratuita y en español» · «Otra página: sobre tu club, tu banda o una receta» · «Un sitio web: une varias páginas con enlaces» · «Practica: mejor 20 min diarios que 4 horas de golpe».
- **Cierre (8:45), Lámina 38:** Lámina final con un mensaje de cierre. Texto en pantalla: «¡Lo lograste!» «#WebDevBeginners»
