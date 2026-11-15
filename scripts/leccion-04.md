# Lección 4: Introducción a CSS

_(Contenido para los instructores)_

**Objetivo:** Al terminar, el estudiante puede escribir una regla de CSS (selector, propiedad y valor) y usarla para cambiar el color de fondo, el color del texto, el tipo de letra, la alineación y el estilo de un elemento con una clase.

**Palabras nuevas:** CSS, regla, selector, propiedad, valor, clase, color hexadecimal, tipo de letra (fuente).

## 1. Estructura de carpetas (GitHub)

```text
/starter-files/leccion-04        # Código de inicio de la lección
├── index.html
└── styles.css

/completed-examples/leccion-04   # Código completo de la lección
├── index.html
└── styles.css
```

## 2. Guion del video (12 minutos)

> Los tiempos son los del audio (unos 11:09). Con las tarjetas de pausa, los Ejecutar y las transiciones de la edición, el video llega a unos 12 minutos. El guion detallado para grabar está en `grabacion/leccion-04.md` (solo para el equipo).

> **(0:00 - 0:48) Introducción**  
> ¡Hola! Te doy la bienvenida a la lección 4 del curso. Hasta ahora tu página tiene todo su contenido: un título, tu foto, tus pasatiempos, tus metas y un enlace. Pero se ve sencilla, como una hoja de tareas: letras negras sobre fondo blanco. Hoy eso cambia. Vas a darle estilo con CSS: colores, tipos de letra y alineación. Piensa en un videojuego: el mapa y los personajes son el contenido, pero sus colores y su ropa son lo que lo hace único. Eso es CSS para tu página. ¡Empecemos!
>
> **(0:48 - 1:42) Una regla de CSS**  
> En CSS todo se escribe con reglas, y una regla tiene tres partes. Primero, el selector, que dice a qué elemento se aplica: aquí, a los títulos h1. Luego, entre llaves, va la propiedad, que dice qué quieres cambiar: el color. Después de los dos puntos va el valor, que dice cómo lo quieres: azul. Y cada línea termina con un punto y coma. Se lee así: a los elementos h1, aplícales el color azul. Es como dar una orden con tres datos: a quién, qué cosa y cómo. Por ejemplo: a mi mochila, el color, rojo.
>
> **(1:42 - 2:19) ¿Dónde se escribe el CSS?**  
> ¿Y dónde se escribe el CSS? En JSFiddle es fácil: en el panel CSS, el de arriba a la derecha. En un sitio web real, el CSS se guarda en un archivo aparte, con extensión punto css, y se conecta con la página con una línea en el head: la etiqueta link. La idea es la misma en los dos lugares: las reglas se escriben igual.
>
> **(2:19 - 3:30) Color de fondo**  
> Aquí está la página de la lección 3, y el panel CSS está vacío. ¡Escribe conmigo! Empecemos por el fondo de toda la página. El selector es body, que representa toda la página. Abro una llave y la cierro. Adentro va la propiedad background-color, que significa color de fondo, seguida de dos puntos. Y el valor es un código de color que empieza con numeral: numeral, f, e, f, 3, c, 7. Y al final, punto y coma. Pulso Ejecutar y… ¡mira! La página cambió a un tono crema. También existen nombres de colores en inglés, como tomato o skyblue, pero con los códigos tienes muchos más tonos.
>
> **(3:30 - 4:10) Códigos de color**  
> Esos códigos se llaman hexadecimales. Después del numeral vienen tres pares de caracteres: el primer par dice cuánto rojo, el segundo cuánto verde y el tercero cuánto azul. Mezclando esas tres luces, la pantalla de tu celular forma todos los colores que ves. No necesitas memorizarlos. En la descripción de este video te dejé una paleta lista para copiar, con cinco colores: fondo crema, título marrón, subtítulos verde azulado, texto oscuro y un amarillo para resaltar.
>
> **(4:10 - 5:20) Colores de los títulos**  
> Ahora los títulos. Debajo de la regla de body escribo h1 y abro y cierro llaves. Adentro: color, dos puntos, numeral, b, 4, 5, 3, 0, 9, y punto y coma. Ejecutar. ¡El título principal ya es marrón! Ahora los subtítulos. Debajo escribo h2 y, adentro, color con el verde azulado: numeral, 0, f, 7, 6, 6, e. Ejecutar. Fíjate: con una sola regla cambiaron los dos subtítulos a la vez. Un selector le habla a todos los elementos de ese tipo. Un consejo importante: elige colores que contrasten con el fondo. Un amarillo clarito sobre crema casi no se distingue, y nadie lo podría leer.
>
> **(5:20 - 6:53) Tipo, tamaño y color de letra**  
> Pasemos a las letras. Vuelvo a la regla de body y, arriba de background-color, escribo font-family, que elige el tipo de letra. Pongo varias opciones separadas por comas: Arial, Helvetica y sans-serif. Si la primera no está en la computadora de quien visita tu página, el navegador usa la siguiente. La última, sans-serif, es el plan de respaldo. Debajo va font-size, el tamaño de la letra: 18 píxeles. Y por último, debajo de background-color, la propiedad color, que es el color del texto: el oscuro de la paleta, numeral, 1, e, 2, 9, 3, b. Ejecutar. Fíjate: como lo escribí en body, toda la página cambió de letra y de tamaño, incluso las listas. Pero los títulos siguen en marrón y en verde, porque sus propias reglas les dan otro color.
>
> **(6:53 - 7:44) Comentarios y orden de las reglas**  
> Tu CSS ya tiene varias reglas; para ordenarlo existen los comentarios: se escriben entre barra asterisco y asterisco barra. Arriba de body escribo: Estilo general de toda la página. Y arriba de h1: Títulos. Ejecutar. No cambió nada, y está bien: los comentarios son notas para ti, el navegador no los muestra. Y un dato útil: si dos reglas dicen cosas distintas sobre lo mismo, gana la que está más abajo. Por eso el orden de tu CSS importa.
>
> **(7:44 - 9:14) Clases**  
> A veces quieres cambiar un solo elemento, y no todos los de un tipo. Por ejemplo, quiero resaltar solo el párrafo que dice Estoy en secundaria, y no el otro. Para eso están las clases. Primero, en el panel HTML, dentro de la etiqueta de apertura de ese párrafo, agrego el atributo class con el nombre destacado. Luego, en el panel CSS, al final, escribo un comentario: Una clase: solo afecta a los elementos que la usan. Y debajo, un punto y el mismo nombre: punto destacado. Adentro, background-color con el amarillo de la paleta: numeral, f, d, e, 6, 8, a. Ejecutar. ¡Mira! Solo ese párrafo tiene fondo amarillo; el otro no cambió. Una clase es como una etiqueta con nombre que les pones a los elementos que quieres estilizar.
>
> **(9:14 - 9:58) Alineación del texto**  
> Una última propiedad: text-align, que controla la alineación del texto. Dentro de la regla de h1, debajo del color, escribo text-align, dos puntos, center. Ejecutar. ¡El título quedó centrado! También existen left, a la izquierda, y right, a la derecha. Prueba rápida: cambio center por right y pulso Ejecutar. Se fue a la derecha. Lo dejo en center, pulso Ejecutar, y listo.
>
> **(9:58 - 10:31) Pausa y prueba**  
> ¡Te toca! Pausa el video y dale tu propio estilo a tu página. Cambia el fondo y el color de los títulos, elige otro tipo de letra y crea una clase para destacar algo que te guste. Si algo no cambia, revisa que cada línea termine con punto y coma y que las llaves estén cerradas. Cuando termines, sigue con el video.
>
> **(10:31 - 11:09) Resumen**  
> ¡Lo lograste! Hoy aprendiste que una regla de CSS tiene selector, propiedad y valor. Cambiaste el color de fondo, el color del texto y el tipo de letra, y creaste una clase con punto. Y recuerda: cuida siempre el contraste, para que el texto se lea bien. En la próxima lección vas a juntar todo lo que aprendiste para armar tu página de perfil completa. ¡Nos vemos ahí!

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 20:** Lámina de título. Sin texto añadido en pantalla.
- **Una regla de CSS (0:48), Lámina 21:** Lámina con una regla de CSS: `h1 { color: blue; }`. Cada parte va en su color y se resalta cuando se nombra. Sin texto añadido en pantalla.
- **¿Dónde se escribe el CSS? (1:42), Lámina 22, con el editor (JSFiddle) en medio:** Lámina con dos caminos: «En JSFiddle: en el panel CSS del editor» y «En un sitio real: en un archivo `.css`, conectado con `<link>` en el `head`». Al decir «el de arriba a la derecha» se muestra unos 4 segundos JSFiddle con el fiddle de inicio y una flecha al panel CSS (vacío); luego se vuelve a la lámina. Sin texto añadido en pantalla. Anotaciones: flecha «Panel CSS» en el editor y círculo sobre «`<link>` en el `head`» en la lámina.
- **Color de fondo (2:19), Editor (JSFiddle), sin lámina:** JSFiddle con la página de la lección 3 y el panel CSS vacío. Se escribe `body { background-color: #fef3c7; }` y se pulsa Ejecutar: el fondo cambia a crema. Texto en pantalla: «`body` = toda la página» · «`background-color` = color de fondo». Zoom al valor.
- **Códigos de color (3:30), Lámina 23 y luego Lámina 24:** Lámina 23: «Códigos de color», con `#b45309` partido en `b4`, `53` y `09`. Después, la Lámina 24 con la paleta de cinco colores. Sin texto añadido en pantalla.
- **Colores de los títulos (4:10), Editor (JSFiddle), sin lámina:** Debajo de la regla de `body` se escribe `h1 { color: #b45309; }` y se pulsa Ejecutar: el título cambia a marrón. Luego `h2 { color: #0f766e; }` y Ejecutar: cambian los dos subtítulos. Texto en pantalla: «Un selector, todos los elementos de ese tipo» · «Contraste: el texto debe poder leerse».
- **Tipo, tamaño y color de letra (5:20), Editor (JSFiddle), sin lámina:** Dentro de `body`, arriba de `background-color`, se agregan `font-family: Arial, Helvetica, sans-serif;` y `font-size: 18px;`, y debajo, `color: #1e293b;`. Se pulsa Ejecutar: todo el texto cambia de letra y de tamaño; los títulos mantienen su color. Texto en pantalla: «`font-family` = tipo de letra» · «Si no existe el primero, usa el siguiente» · «`color` = color del texto». Anotación: subrayar `sans-serif` como «plan de respaldo».
- **Comentarios y orden de las reglas (6:53), Editor (JSFiddle), sin lámina:** Se escriben dos comentarios: `/* Estilo general de toda la página */` arriba de `body` y `/* Títulos */` arriba de `h1`. Se pulsa Ejecutar: la página no cambia. Texto en pantalla: «Comentarios en CSS: `/* ... */`» · «Si dos reglas chocan, gana la que está más abajo».
- **Clases (7:44), Editor (JSFiddle), sin lámina:** En el panel HTML se agrega `class="destacado"` al párrafo «Estoy en secundaria…». En el panel CSS, al final, se escriben el comentario `/* Una clase: solo afecta a los elementos que la usan */` y `.destacado { background-color: #fde68a; }`. Se pulsa Ejecutar: solo ese párrafo cambia. Texto en pantalla: «Clase: en CSS lleva un punto antes del nombre» · «En el HTML: `class="destacado"`». Anotación: flecha entre el atributo y la regla.
- **Alineación del texto (9:14), Editor (JSFiddle), sin lámina:** Dentro de `h1`, debajo de `color`, se agrega `text-align: center;` y se pulsa Ejecutar: el título se centra. Prueba rápida con `right` y vuelta a `center`. Texto en pantalla: «`text-align`: `left`, `center`, `right`».
- **Pausa y prueba (9:58), Lámina 25:** Tarjeta de pausa de 5 segundos. Sin texto añadido en pantalla.
- **Resumen (10:31), Lámina 26:** Lámina de resumen con cuatro tarjetas. Sin texto añadido en pantalla.

## 4. Pregunta para pensar

Si cambias el color en la regla de `body`, ¿qué elementos cambian? ¿Y si lo cambias en `h1`?
