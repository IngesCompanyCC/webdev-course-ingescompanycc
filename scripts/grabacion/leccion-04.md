# Lección 4: Introducción a CSS (12 minutos)

> Guion detallado para grabar. La versión para presentar está en [../leccion-04.md](../leccion-04.md).

**Objetivo:** al terminar, el estudiante puede escribir una regla de CSS (selector, propiedad y valor) y usarla para cambiar el color de fondo, el color del texto, el tipo de letra, la alineación y el estilo de un elemento con una clase.

**Fiddle de inicio:** TODO (enlace de JSFiddle con el código de [`starter-files/leccion-04/`](../../starter-files/leccion-04/); trae la página de la lección 3 y el panel CSS vacío)

**Código terminado:** [`completed-examples/leccion-04/`](../../completed-examples/leccion-04/)

**Palabras nuevas de la lección:** CSS, regla, selector, propiedad, valor, clase, color hexadecimal, tipo de letra (fuente).

**Antes de grabar:**

- Abre la presentación [webdev-course.pptx](../../slides/webdev-course.pptx). La columna **Lámina** dice cuál mostrar en cada escena; donde dice «Editor (JSFiddle), sin lámina» se graba solo la pantalla del editor, sin diapositiva.
- Ten lista una pequeña paleta de colores en la descripción (ver abajo) para que el estudiante pueda copiar los valores.
- El tipo de letra es `Arial`, que está en casi todas las computadoras: así no se necesita instalar ni cargar nada.
- Haz zoom al panel CSS: las llaves y los puntos y comas deben leerse bien.

| Tiempo | Lámina | En pantalla | Texto en pantalla y anotaciones | Narración (en off) |
|---|---|---|---|---|
| 0:00 | **Lám. 20** | Lámina de título. | **Texto:** «Lección 4 · Introducción a CSS» | «Hasta ahora tu página tiene todo su contenido, pero se ve muy sencilla. Hoy vas a darle estilo con CSS: colores, letras y alineación. Vas a ver cómo, con muy pocas líneas, la página cambia por completo.» |
| 0:45 | **Lám. 21** | Lámina con una regla de CSS: `h1 { color: blue; }`. Cada parte va en su color y debajo hay tres etiquetas: selector, propiedad y valor. | **Texto:** «Selector: ¿a qué elemento?» · «Propiedad: ¿qué cambio?» · «Valor: ¿cómo?». | «Una regla de CSS tiene tres partes. Primero, el selector, que dice a qué elemento se aplica: aquí, a los títulos h1. Luego, entre llaves, va la propiedad, que dice qué quieres cambiar: el color. Después de dos puntos va el valor, que dice cómo: azul. Y cada línea termina con un punto y coma. Se lee así: a los elementos h1, aplícales el color azul.» |
| 2:15 | **Lám. 22** | Lámina con dos caminos: «En JSFiddle: panel CSS» y «En un sitio real: archivo `.css` con `<link rel="stylesheet" href="styles.css">`». | **Texto:** «¿Dónde se escribe el CSS?» **Anotación:** señalar la etiqueta `link` dentro del `head`. | «¿Dónde se escribe el CSS? En JSFiddle, en el panel CSS. En un sitio web real, se guarda en un archivo aparte con extensión punto css, y se conecta con la página mediante una línea en el `head`. La idea es la misma: las reglas son las mismas en los dos lugares.» |
| 3:15 | Editor (JSFiddle), sin lámina | JSFiddle con la página de la lección 3 y el panel CSS vacío. Se escribe `body { background-color: #fef3c7; }`. El fondo cambia a crema. | **Texto:** «`body` = toda la página» · «`background-color` = color de fondo». **Zoom** al valor. | «Empecemos por el fondo de toda la página. El selector es body. La propiedad es `background-color`, que significa color de fondo. Y el valor es un código de color que empieza con numeral. Mira: la página cambió a un tono crema. También puedes usar nombres de colores, como `tomato` o `skyblue`.» |
| 4:15 | **Lám. 23** y luego **Lám. 24** | Lámina corta: «Códigos de color». Se muestra `#b45309` partido en `b4`, `53`, `09`. Después, la Lám. 24 con la paleta de cinco colores. | **Texto:** «`#` + rojo + verde + azul». «Copia los códigos de la descripción». | «Esos códigos se llaman hexadecimales. Son tres pares de caracteres: cuánto rojo, cuánto verde y cuánto azul. No necesitas memorizarlos: en la descripción de este video te dejé una paleta lista para copiar.» |
| 4:45 | Editor (JSFiddle), sin lámina | Se escribe `h1 { color: #b45309; }`. El título cambia de color. Luego `h2 { color: #0f766e; }`. | **Texto:** «Un selector por tipo de elemento». «Contraste: el texto debe poder leerse». | «Ahora los títulos. Con el selector h1 cambio el color del título principal y con h2, el de los subtítulos. Un consejo: elige colores que contrasten con el fondo. Si el texto casi no se distingue, nadie lo va a poder leer.» |
| 6:00 | Editor (JSFiddle), sin lámina | Se agrega a `body`: `font-family: Arial, Helvetica, sans-serif;` y `font-size: 18px;`. Todo el texto cambia. | **Texto:** «`font-family` = tipo de letra» · «Si no existe el primero, usa el siguiente». **Anotación:** subrayar `sans-serif` como «plan de respaldo». | «Pasemos a las letras. `font-family` elige el tipo de letra. Escribo varias opciones separadas por comas: si la primera no está en la computadora de quien visita tu página, usa la siguiente. La última, `sans-serif`, es el plan de respaldo. Y con `font-size` cambio el tamaño. Fíjate que, al escribirlo en body, todo el texto de la página cambió.» |
| 7:30 | Editor (JSFiddle), sin lámina | Se escribe un comentario: `/* Títulos */`. Lámina corta con la idea «la regla más abajo gana si hay choque». | **Texto:** «Comentarios en CSS: `/* ... */`» · «Si dos reglas chocan, gana la que está más abajo». | «En CSS también hay comentarios, y se escriben entre barra y asterisco. Sirven para ordenar tu código. Y un dato útil: si dos reglas dicen cosas distintas sobre lo mismo, gana la que está más abajo.» |
| 8:15 | Editor (JSFiddle), sin lámina | Se agrega `class="destacado"` al párrafo «Estoy en secundaria…». En CSS: `.destacado { background-color: #fde68a; }`. Solo ese párrafo cambia. | **Texto:** «Clase: se usa un punto antes del nombre». «Etiqueta: `class="destacado"`». **Anotación:** unir con una flecha el atributo y la regla. | «A veces quieres cambiar solo un elemento, y no todos los de un tipo. Para eso están las clases. Primero, en el HTML le agrego al párrafo el atributo `class` con el nombre `destacado`. Luego, en CSS, escribo un punto y el mismo nombre. Mira: solo ese párrafo cambió. Una clase es un nombre que les asignas a los elementos que quieres estilizar.» |
| 9:45 | Editor (JSFiddle), sin lámina | Se agrega `text-align: center;` al `h1`. El título se centra. | **Texto:** «`text-align`: `left`, `center`, `right`». | «Una última propiedad: `text-align` controla la alineación del texto. Con `center`, el título queda centrado. Puedes probar también `left` y `right`.» |
| 10:30 | **Lám. 25** | Tarjeta de pausa de 5 segundos con cuenta regresiva. | **Texto:** «Pausa el video y prueba» · «Tómate el tiempo que necesites»: «1. Cambia el fondo. 2. Cambia el color de los títulos. 3. Elige otro tipo de letra. 4. Crea una clase y úsala en un elemento». | «Es tu turno. Pausa el video y dale tu estilo: cambia el fondo, el color de los títulos, el tipo de letra y crea una clase para destacar algo. Si algo no cambia, revisa que cada línea termine con punto y coma y que las llaves estén cerradas. Cuando termines, continúa.» |
| 11:30 | **Lám. 26** | Lámina de resumen. | **Texto:** «Regla = selector + propiedad + valor» · «Clases: `.nombre`» · «Cuida el contraste». | «Hoy aprendiste que una regla de CSS tiene selector, propiedad y valor; cambiaste colores, letras y alineación, y creaste una clase. En la próxima lección vas a juntar todo para armar tu página de perfil completa.» |

**Código de la lección:**

HTML (solo un cambio respecto a la lección 3: el párrafo lleva la clase `destacado`):

```html
<p class="destacado">Estoy en secundaria y me encanta aprender cosas nuevas.</p>
```

CSS (panel CSS de JSFiddle):

```css
/* Estilo general de toda la página */
body {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 18px;
  background-color: #fef3c7;
  color: #1e293b;
}

/* Títulos */
h1 {
  color: #b45309;
  text-align: center;
}

h2 {
  color: #0f766e;
}

/* Una clase: solo afecta a los elementos que la usan */
.destacado {
  background-color: #fde68a;
}
```

**Pregunta para pensar:** si cambias el color en la regla de `body`, ¿qué elementos cambian? ¿Y si lo cambias en `h1`?

**Paleta para copiar (va en la descripción):**

| Uso | Código |
|---|---|
| Fondo crema | `#fef3c7` |
| Título marrón | `#b45309` |
| Subtítulos verde azulado | `#0f766e` |
| Texto oscuro | `#1e293b` |
| Resaltado amarillo | `#fde68a` |

**Descripción para YouTube:**

> Lección 4 del curso Fundamentos de Desarrollo Web: HTML y CSS. Aprende a darle color y estilo a tu página.
> Practica aquí, sin instalar nada: TODO-enlace-jsfiddle
> Paleta para copiar: fondo #fef3c7 · títulos #b45309 · subtítulos #0f766e · texto #1e293b · resaltado #fde68a
> Reto: cambia el fondo, el color de los títulos, el tipo de letra y crea una clase.
> #WebDevBeginners

**Revisión antes de subir:**

- [ ] Dura entre 5 y 15 minutos.
- [ ] Texto en pantalla, anotaciones y narración en off en cada escena.
- [ ] Los códigos de color de la paleta coinciden con los del video.
- [ ] Se explica el contraste (que el texto se pueda leer).
- [ ] Sin nombres, caras ni logos del equipo.
- [ ] Se sube como **no listado**, con el enlace al fiddle en la descripción.
