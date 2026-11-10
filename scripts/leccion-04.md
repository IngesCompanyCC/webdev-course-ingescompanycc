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

> **(0:00 - 0:45) Introducción**  
> Hasta ahora tu página tiene todo su contenido, pero se ve muy sencilla. Hoy vas a darle estilo con CSS: colores, letras y alineación. Vas a ver cómo, con muy pocas líneas, la página cambia por completo.
>
> **(0:45 - 2:15) Una regla de CSS**  
> Una regla de CSS tiene tres partes. Primero, el selector, que dice a qué elemento se aplica: aquí, a los títulos h1. Luego, entre llaves, va la propiedad, que dice qué quieres cambiar: el color. Después de dos puntos va el valor, que dice cómo: azul. Y cada línea termina con un punto y coma. Se lee así: a los elementos h1, aplícales el color azul.
>
> **(2:15 - 3:15) ¿Dónde se escribe el CSS?**  
> ¿Dónde se escribe el CSS? En JSFiddle, en el panel CSS. En un sitio web real, se guarda en un archivo aparte con extensión punto css, y se conecta con la página mediante una línea en el `head`. La idea es la misma: las reglas son las mismas en los dos lugares.
>
> **(3:15 - 4:15) Color de fondo**  
> Empecemos por el fondo de toda la página. El selector es body. La propiedad es `background-color`, que significa color de fondo. Y el valor es un código de color que empieza con numeral. Mira: la página cambió a un tono crema. También puedes usar nombres de colores, como `tomato` o `skyblue`.
>
> **(4:15 - 4:45) Códigos de color**  
> Esos códigos se llaman hexadecimales. Son tres pares de caracteres: cuánto rojo, cuánto verde y cuánto azul. No necesitas memorizarlos: en la descripción de este video te dejé una paleta lista para copiar.
>
> **(4:45 - 6:00) Colores de los títulos**  
> Ahora los títulos. Con el selector h1 cambio el color del título principal y con h2, el de los subtítulos. Un consejo: elige colores que contrasten con el fondo. Si el texto casi no se distingue, nadie lo va a poder leer.
>
> **(6:00 - 7:30) Tipo y tamaño de letra**  
> Pasemos a las letras. `font-family` elige el tipo de letra. Escribo varias opciones separadas por comas: si la primera no está en la computadora de quien visita tu página, usa la siguiente. La última, `sans-serif`, es el plan de respaldo. Y con `font-size` cambio el tamaño. Por último, con `color` elijo el color del texto: el oscuro de la paleta, que se lee bien sobre el crema. Fíjate que, al escribirlo en body, todo el texto de la página cambió.
>
> **(7:30 - 8:15) Comentarios y orden de las reglas**  
> En CSS también hay comentarios, y se escriben entre barra y asterisco. Sirven para ordenar tu código. Y un dato útil: si dos reglas dicen cosas distintas sobre lo mismo, gana la que está más abajo.
>
> **(8:15 - 9:45) Clases**  
> A veces quieres cambiar solo un elemento, y no todos los de un tipo. Para eso están las clases. Primero, en el HTML le agrego al párrafo el atributo `class` con el nombre `destacado`. Luego, en CSS, escribo un punto y el mismo nombre. Mira: solo ese párrafo cambió. Una clase es un nombre que les asignas a los elementos que quieres estilizar.
>
> **(9:45 - 10:30) Alineación del texto**  
> Una última propiedad: `text-align` controla la alineación del texto. Con `center`, el título queda centrado. Puedes probar también `left` y `right`.
>
> **(10:30 - 11:30) Pausa y prueba**  
> Es tu turno. Pausa el video y dale tu estilo: cambia el fondo, el color de los títulos, el tipo de letra y crea una clase para destacar algo. Si algo no cambia, revisa que cada línea termine con punto y coma y que las llaves estén cerradas. Cuando termines, continúa.
>
> **(11:30 - 12:00) Resumen**  
> Hoy aprendiste que una regla de CSS tiene selector, propiedad y valor; cambiaste colores, letras y alineación, y creaste una clase. En la próxima lección vas a juntar todo para armar tu página de perfil completa.

## 3. Sugerencias multimedia

- **Introducción (0:00), Lámina 20:** Lámina de título. Texto en pantalla: «Lección 4 · Introducción a CSS»
- **Una regla de CSS (0:45), Lámina 21:** Lámina con una regla de CSS: `h1 { color: blue; }`. Cada parte va en su color y debajo hay tres etiquetas: selector, propiedad y valor. Texto en pantalla: «Selector: ¿a qué elemento?» · «Propiedad: ¿qué cambio?» · «Valor: ¿cómo?» · «Cada línea termina con punto y coma (;)».
- **¿Dónde se escribe el CSS? (2:15), Lámina 22:** Lámina con dos caminos: «En JSFiddle: en el panel CSS del editor» y «En un sitio real: en un archivo `.css`, conectado con `<link>` en el `head`». Texto en pantalla: «¿Dónde se escribe el CSS?» Anotación: señalar «`<link>` en el `head`».
- **Color de fondo (3:15), Editor (JSFiddle), sin lámina:** JSFiddle con la página de la lección 3 y el panel CSS vacío. En el panel CSS se escribe `body { background-color: #fef3c7; }` y se pulsa Ejecutar. El fondo cambia a crema. Texto en pantalla: «`body` = toda la página» · «`background-color` = color de fondo». Zoom al valor.
- **Códigos de color (4:15), Lámina 23 y luego Lámina 24:** Lámina corta: «Códigos de color». Se muestra `#b45309` partido en `b4`, `53`, `09`. Después, la Lám. 24 con la paleta de cinco colores. Texto en pantalla: «`#` + rojo + verde + azul». «Copia los códigos de la descripción».
- **Colores de los títulos (4:45), Editor (JSFiddle), sin lámina:** Debajo de la regla de `body` se escribe `h1 { color: #b45309; }` y se pulsa Ejecutar: el título cambia de color. Luego, debajo, `h2 { color: #0f766e; }` y Ejecutar: cambian los subtítulos. Texto en pantalla: «Un selector por tipo de elemento». «Contraste: el texto debe poder leerse».
- **Tipo y tamaño de letra (6:00), Editor (JSFiddle), sin lámina:** Dentro de `body`, arriba de `background-color`, se agregan `font-family: Arial, Helvetica, sans-serif;` y `font-size: 18px;`, y debajo de `background-color`, `color: #1e293b;`. Se pulsa Ejecutar: todo el texto cambia. Texto en pantalla: «`font-family` = tipo de letra» · «Si no existe el primero, usa el siguiente» · «`color` = color del texto». Anotación: subrayar `sans-serif` como «plan de respaldo».
- **Comentarios y orden de las reglas (7:30), Editor (JSFiddle), sin lámina:** Se escriben dos comentarios: `/* Estilo general de toda la página */` arriba de `body` y `/* Títulos */` arriba de `h1`. Se pulsa Ejecutar: la página no cambia, porque los comentarios no se ven. Texto en pantalla: «Comentarios en CSS: `/* ... */`» · «Si dos reglas chocan, gana la que está más abajo».
- **Clases (8:15), Editor (JSFiddle), sin lámina:** En el panel HTML se agrega `class="destacado"` al párrafo «Estoy en secundaria…». En el panel CSS, al final, se escriben el comentario `/* Una clase: solo afecta a los elementos que la usan */` y `.destacado { background-color: #fde68a; }`. Se pulsa Ejecutar: solo ese párrafo cambia. Texto en pantalla: «Clase: se usa un punto antes del nombre». «Etiqueta: `class="destacado"`». Anotación: unir con una flecha el atributo y la regla.
- **Alineación del texto (9:45), Editor (JSFiddle), sin lámina:** Dentro de `h1`, debajo de `color`, se agrega `text-align: center;` y se pulsa Ejecutar. El título se centra. Texto en pantalla: «`text-align`: `left`, `center`, `right`».
- **Pausa y prueba (10:30), Lámina 25:** Tarjeta de pausa de 5 segundos con cuenta regresiva. Texto en pantalla: «Pausa y prueba» · «Tómate el tiempo que necesites» · «Cambia el fondo y el color de los títulos» · «Elige otro tipo de letra» · «Crea una clase y úsala en un elemento».
- **Resumen (11:30), Lámina 26:** Lámina de resumen con cuatro tarjetas. Texto en pantalla: «Regla: selector, propiedad y valor, entre llaves» · «Color y letra: `background-color`, `color` y `font-family`» · «Clases: en CSS llevan un punto: `.destacado`» · «Contraste: texto legible sobre su fondo».

## 4. Pregunta para pensar

Si cambias el color en la regla de `body`, ¿qué elementos cambian? ¿Y si lo cambias en `h1`?
