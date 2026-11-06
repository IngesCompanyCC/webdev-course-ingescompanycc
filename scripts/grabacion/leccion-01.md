# Lección 1: ¿Qué es un sitio web? (5 minutos)

> Guion detallado para grabar. La versión para presentar está en [../leccion-01.md](../leccion-01.md).

**Duración estimada:** 5 minutos y 15 segundos (la última escena incluye un cierre pausado).

**Objetivo:** al terminar, el estudiante puede explicar con sus palabras qué es un sitio web, decir para qué sirven HTML y CSS, y ver en un editor en línea la diferencia entre una página con estilo y una sin estilo.

**Fiddle de inicio:** TODO (enlace de JSFiddle con el código de [`starter-files/leccion-01/`](../../starter-files/leccion-01/))

**Código terminado:** [`completed-examples/leccion-01/`](../../completed-examples/leccion-01/) (esta lección solo explora; el ejemplo es el mismo del fiddle de inicio).

**Palabras nuevas de la lección** (decirlas siempre igual): sitio web, página web, navegador, dirección, solicitud, servidor, HTML, CSS, editor en línea.

**Antes de grabar:**

- Abre la presentación [webdev-course.pptx](../../slides/webdev-course.pptx). La columna **Lámina** dice cuál mostrar en cada escena; donde dice «Editor (JSFiddle), sin lámina» se graba solo la pantalla del editor, sin diapositiva.
- Abre el fiddle de inicio en JSFiddle y haz zoom del navegador (`Ctrl` y `+`) hasta que el código se lea bien en un video de 1080p.
- Ten a mano una pestaña con una página cualquiera (por ejemplo, la de un colegio o un blog) para la escena de 0:25. No muestres nombres ni logos del equipo.

| Tiempo | Lámina | En pantalla | Texto en pantalla y anotaciones | Narración (en off) |
|---|---|---|---|---|
| 0:00 | **Lám. 1** (portada del curso) y **Lám. 2** | Portada del curso y portada de la lección 1. | **Texto:** «Lección 1 · ¿Qué es un sitio web?» | «Hola, te doy la bienvenida. En este curso vas a crear tu propia página web, a tu ritmo y desde cero y sin instalar nada: solo necesitas un navegador. Empecemos por lo básico: ¿qué es, de verdad, un sitio web?» |
| 0:25 | Navegador, sin lámina | Una página web cualquiera, sin nombres ni logos del equipo (por ejemplo, la portada de MDN Web Docs). No se muestra la página de YouTube, porque deja ver el nombre del canal. Acercamiento a la barra de direcciones. | **Anotación:** círculo rojo sobre la dirección. **Texto:** «Un sitio web = páginas conectadas». | «Las páginas web están por todas partes: en tu colegio, en las tiendas, en los blogs y en los periódicos. Un sitio web es un conjunto de páginas conectadas entre sí por enlaces. Y cada página tiene su propia dirección, como esta que ves aquí arriba.» |
| 1:10 | **Lám. 3** | Lámina con el ciclo de tres pasos: solicitud, respuesta y la página en pantalla. Al editar el video se puede resaltar cada paso cuando se nombra. | **Texto (uno por paso):** «1. El navegador envía una solicitud» · «2. El servidor responde con los archivos» · «3. El navegador interpreta el código». | «¿Y cómo llega hasta tu pantalla? Cuando escribes una dirección o haces clic en un enlace, tu navegador envía una solicitud. La recibe un servidor: una computadora donde están guardados los archivos del sitio. El servidor responde enviando esos archivos, y tu navegador los interpreta y te muestra la página.» |
| 2:10 | **Lám. 4** | Lámina con tres columnas: HTML (contenido y estructura), CSS (colores, letras y espacios) y el navegador, que junta los dos. | **Texto:** «HTML = el contenido y la estructura» · «CSS = el estilo» · «El navegador junta HTML y CSS y muestra la página». | «Esos archivos están escritos en lenguajes. Hoy vas a conocer dos. HTML define el contenido y la estructura: qué hay en la página, como títulos, párrafos, imágenes y enlaces. CSS define la presentación: cómo se ve, con colores, letras y espacios. Y el navegador junta los dos: lee el HTML, le aplica el CSS y te muestra la página terminada.» |
| 3:10 | Editor (JSFiddle), sin lámina | JSFiddle con el fiddle de inicio abierto. Se ven los paneles HTML, CSS, JavaScript y Result, y el botón Run. | **Anotación:** flechas que señalan «HTML», «CSS», «Result» y el botón «Run». **Texto:** «JSFiddle: un editor en línea y gratuito» · «Run = ver el resultado». | «Veámoslo en la práctica. Esto es JSFiddle, un editor en línea: funciona desde el navegador y no hace falta instalar nada. Aquí hay un panel para escribir HTML, otro para escribir CSS y una zona, Result, donde aparece el resultado. El panel de JavaScript no lo usamos en este curso. Cada vez que cambies algo, pulsa Run, arriba a la izquierda, o Control Enter, y el resultado se actualiza. Fíjate en el HTML: tiene un título, dos párrafos y una lista. Y en el CSS están los colores y la forma de las casillas.» |
| 3:40 | Editor (JSFiddle), sin lámina | Se hace clic en el panel CSS, `Ctrl + A` para seleccionar todo, se borra y se pulsa **Run**. El resultado cambia a una página sin estilo. Luego `Ctrl + Z` recupera el CSS y se pulsa **Run** otra vez. | **Anotación:** resaltar «antes» y «después». **Texto:** «Mismo contenido, sin CSS». | «Mira qué pasa si borro todo el CSS y pulso Run. Es la misma página y tiene el mismo contenido, pero ahora se ve sencilla: letras negras sobre fondo blanco. Y si recupero el CSS con Control Z y pulso Run, vuelven los colores. HTML define el contenido y CSS, la presentación.» |
| 4:20 | **Lám. 5** | Tarjeta de pausa de 5 segundos con cuenta regresiva. | **Texto:** «Pausa el video y prueba» · «Tómate el tiempo que necesites»: «Abre el enlace de la descripción, borra el CSS, pulsa Run y mira qué cambia. Recupéralo con Ctrl + Z (en Mac, Cmd + Z)». | «Ahora te toca a ti. Pausa el video, abre el enlace de la descripción, borra el CSS, pulsa Run y observa qué cambia. Si quieres volver atrás, usa Control Z. No puedes dañar nada: el fiddle es solo para practicar. Cuando termines, sigue con el video.» |
| 4:45 | **Lám. 6** | Lámina de resumen con tres puntos. | **Texto:** «1. Un sitio web son páginas conectadas» · «2. HTML define el contenido» · «3. CSS define la presentación». | «Hoy aprendiste tres cosas: un sitio web es un conjunto de páginas conectadas, HTML define el contenido y CSS define la presentación. En la próxima lección vas a escribir tu primera página en HTML. Nos vemos allá.» |

**Pregunta para pensar (se puede poner en la descripción):** si una página se ve bien pero sus letras no se leen, ¿el problema está en el HTML o en el CSS?

**Descripción para YouTube:**

> Lección 1 del curso Fundamentos de Desarrollo Web: HTML y CSS. Descubre qué es un sitio web y para qué sirven HTML y CSS.
> Practica aquí, sin instalar nada: TODO-enlace-jsfiddle
> Reto: borra el CSS del fiddle y mira qué cambia. Recupéralo con Ctrl + Z.
> #WebDevBeginners

**Revisión antes de subir** (de la rúbrica del enunciado):

- [ ] Dura entre 5 y 15 minutos.
- [ ] Hay texto en pantalla, anotaciones y narración en off.
- [ ] El texto del editor se lee sin esfuerzo (zoom).
- [ ] No aparecen nombres, caras ni logos del equipo.
- [ ] No hay términos mal traducidos (ver el Anexo C del enunciado).
- [ ] El video se sube como **no listado** y el enlace al fiddle va en la descripción.
