# Lección 5: Proyecto: tu página de perfil

_(Contenido para los instructores)_

**Objetivo:** Al terminar, el estudiante puede combinar HTML y CSS para armar una página de perfil personal: estructura con etiquetas con significado, tarjeta centrada, borde, esquinas redondeadas, imágenes redondas y colores propios.

**Palabras nuevas:** etiqueta con significado (semántica), `header`, `main`, `section`, `footer`, espacio interno (`padding`), espacio externo (`margin`), borde (`border`), esquinas redondeadas (`border-radius`).

## 1. Estructura de carpetas (GitHub)

```text
/starter-files/leccion-05        # Código de inicio de la lección
├── index.html
└── styles.css

/completed-examples/leccion-05   # Código completo de la lección
├── index.html
└── styles.css

/starter-files/assets            # Imágenes de la lección (se enlazan con su dirección completa)
├── avatar.png
└── mascota.png
```

## 2. Guion del video (15 minutos)

> Los tiempos son los del audio (unos 13:51). Con las tarjetas de pausa, los Ejecutar y las transiciones de la edición, el video llega a unos 15 minutos. El guion detallado para grabar está en `grabacion/leccion-05.md` (solo para el equipo).

> **(0:00 - 0:48) El resultado**  
> ¡Hola! Te doy la bienvenida a la lección 5. Llegó el momento de juntar todo lo que aprendiste. Hoy vas a construir una página de perfil completa: con tu foto, tus datos, tus pasatiempos y mucho estilo. Esto que ves es el resultado: una tarjeta centrada, con borde, esquinas redondeadas y fotos redondas, como el perfil de una app. Vas a usar casi todo lo del curso: HTML para la estructura y CSS para el estilo. Al final de esta lección va a ser tuya. ¡Empecemos!
>
> **(0:48 - 1:41) El boceto**  
> Antes de escribir código, quienes hacen páginas web dibujan un boceto, como el plano de una casa. Aquí tenemos: arriba, la foto y el nombre; en el medio, varias secciones; y abajo, un pie con un enlace. Cada parte del boceto va a ser una etiqueta: la cabecera será header; cada sección, section; y el pie, footer. Dibujar primero te ahorra tiempo: sabes qué vas a construir antes de empezar. Puedes hacerlo en una hoja, con lápiz; quienes diseñan apps y videojuegos también empiezan así. Fíjate: el boceto no tiene colores ni detalles; eso llega después, con CSS.
>
> **(1:41 - 3:11) La cabecera**  
> Vamos al editor: los dos paneles están vacíos. ¡Escribe conmigo! Empecemos por la estructura. Primero, una etiqueta main, que envuelve el contenido principal. Le pongo la clase perfil, que usaremos después en el CSS. Como viste en la lección 4 con destacado, una clase es un nombre que tú eliges. Adentro va un header, la cabecera. Ahí pongo la foto, con la clase foto y su texto alternativo, como en la lección 3; el nombre, Alex, en un h1; y una frase corta, en un párrafo. Ejecutar. La foto se ve enorme y todo está sin estilo; no te preocupes, eso lo arreglamos con CSS. Fíjate que main y header no cambian cómo se ve la página, pero le dan un significado: le dicen al navegador, y a quienes usan lectores de pantalla, qué es cada parte. Por eso se llaman etiquetas semánticas, es decir, con significado.
>
> **(3:11 - 4:54) Secciones y pie de página**  
> Ahora, las secciones. Debajo del header escribo la primera section, con su título h2, Sobre mí, y un párrafo. La segunda, Mis pasatiempos, con una lista ul de tres elementos. Les puse emojis, que en HTML se escriben igual que cualquier letra. Fíjate en la sangría: cada sección va un nivel más adentro que main. La tercera, Mi mascota, con la foto de Miso y la clase mascota. Y al final, un footer, el pie de la página, con el enlace a MDN y la frase Hecho con HTML y CSS. Ejecutar. Mira cómo todo lo que aprendiste está aquí: títulos, párrafos, listas, imágenes y enlaces. Todavía se ve sencilla, pero el contenido ya está completo. ¿Y por qué usar section? Porque cada parte queda agrupada, como los capítulos de un libro, y después es fácil moverla o darle estilo.
>
> **(4:54 - 6:07) Estilo general**  
> Ahora le toca al CSS. En el panel CSS empiezo con un comentario: 1, Estilo general de la página. Debajo, la regla de body: la letra Arial, el tamaño de 18 píxeles, un fondo azul claro y un color de texto oscuro. También quito el margen que el navegador pone por defecto, con margin cero, y agrego un espacio interno de 24 píxeles, con padding, para que nada quede pegado al borde. Ejecutar. ¡Fondo azul claro y letra nueva! Todo lo que escribes en body lo heredan los demás elementos. Elegí el azul claro porque combina con el verde azulado que usaremos en los bordes y los títulos.
>
> **(6:07 - 8:13) La caja y la tarjeta centrada**  
> Antes de seguir, una idea clave de CSS: todo elemento es una caja. Adentro está el contenido. Alrededor, el espacio interno, que se llama padding. Luego viene el borde, border. Y afuera, el espacio externo, que es el margen, margin. Piensa en un regalo: el regalo es el contenido, el relleno de papel es el padding, la caja es el borde, y el espacio entre esa caja y las demás es el margen. Volvamos al editor. Escribo el comentario 2, La tarjeta, y la regla punto perfil, para la clase de main. Le doy un ancho máximo de 560 píxeles con max-width. Para centrarla uso margin con cero auto: el cero es para arriba y abajo, y auto reparte por igual los lados. Ejecutar. Prueba rápida: si borro el ancho máximo y pulso Ejecutar, la tarjeta ocupa todo el ancho y no se nota el centrado. Lo recupero con Control Z. Ahora agrego un espacio interno de 24 píxeles, fondo blanco, un borde de 4 píxeles verde azulado, esquinas redondeadas con border-radius y el texto centrado. Ejecutar. ¡Ya parece una tarjeta de verdad! El borde se escribe con tres datos en una línea: el grosor, 4 píxeles; el tipo, solid, que es una línea continua; y el color.
>
> **(8:13 - 9:33) Imágenes redondas**  
> Ahora, las fotos. Escribo el comentario 3, Las imágenes redondas. Como las dos imágenes comparten el mismo estilo, las escribo juntas, separadas por una coma: punto foto, coma, punto mascota. Les doy un borde, y el truco para hacerlas redondas: border-radius igual a 50 por ciento. Y object-fit, cover, que evita que la imagen se deforme. Después le doy a cada una su propio tamaño: la foto, 160 píxeles de ancho y de alto; la mascota, 120. Ejecutar. ¡Dos fotos redondas, como las de perfil en tus apps favoritas! Prueba rápida: en la regla compartida cambio 50 por ciento por 20 píxeles y pulso Ejecutar. Las esquinas quedan apenas redondeadas. Lo regreso a 50 por ciento y pulso Ejecutar.
>
> **(9:33 - 11:21) Los detalles**  
> Ahora los detalles. Comentario 4, Títulos y lista. Pinto el h1 y los h2 con el verde azulado de la paleta. El tamaño de los subtítulos lo escribo en rem, una medida que depende del tamaño de letra de la página: 1.3 rem es un poco más grande que el texto normal, y 0.9 rem, en el pie, un poco más pequeño. En la lista, quito las viñetas con list-style igual a none y el espacio interno que trae por defecto, para que quede centrada; y separo un poco cada elemento con un margen. Comentario 5, Pie de página. Al footer le doy margen arriba, un texto más pequeño y un color gris oscuro; y al enlace, un azul que se lee bien. Ejecutar. Cuida siempre el contraste: el texto tiene que poder leerse con facilidad. Prueba rápida: si cambio el gris del pie por uno muy clarito y pulso Ejecutar… casi no se lee. Lo regreso al gris oscuro y pulso Ejecutar.
>
> **(11:21 - 11:57) Pantallas pequeñas**  
> Un detalle bonito: si achico el panel de resultado, como si fuera la pantalla de un celular… la tarjeta se adapta sola. Eso pasa gracias al ancho máximo que le pusimos: la tarjeta mide como mucho 560 píxeles, pero puede ser más angosta. Hoy mucha gente visita páginas desde el celular, por eso conviene que la tuya se vea bien en pantallas pequeñas.
>
> **(11:57 - 12:31) Pausa y personaliza**  
> ¡Te toca! Pausa el video y arma tu propia página de perfil. Cambia los colores, escribe tus propios pasatiempos y agrega o quita las secciones que quieras: por ejemplo, una con tus comidas o tus series favoritas. Si algo se ve raro, revisa que cada regla tenga sus llaves y cada línea su punto y coma. Cuando termines, vuelve para ver cómo guardarla.
>
> **(12:31 - 13:20) Guardar y compartir**  
> Para guardar tu página en JSFiddle, pulsa Guardar: el ícono de la nube con una flecha, al lado de Ejecutar. Arriba, en la barra de direcciones, aparece un enlace nuevo con tu versión. Así puedes seguir otro día desde donde lo dejaste. Si el editor te pide crear una cuenta y no puedes o no quieres crearla, copia tu HTML y tu CSS en un documento y guárdalo. Algunos sitios piden una edad mínima para crear una cuenta. Y puedes compartir el enlace de tu página con tu familia y tus amistades.
>
> **(13:20 - 13:51) Resumen**  
> ¡Lo lograste! Hoy construiste una página de perfil completa, un proyecto real que puedes mostrar y seguir mejorando. Usaste etiquetas con significado, como header, section y footer; aprendiste el modelo de caja, con padding, border y margin; y centraste, coloreaste y redondeaste. En la última lección vemos los errores más comunes y cómo encontrarlos. ¡Nos vemos ahí!

## 3. Sugerencias multimedia

- **El resultado (0:00), Lámina 27 (unos 3 s) y luego el resultado terminado:** Lámina de título unos 3 segundos y luego la página de perfil terminada, a pantalla completa, con un recorrido del cursor. Sin texto añadido en pantalla.
- **El boceto (0:48), Lámina 28:** Lámina con un boceto de la página: cajas para foto y nombre (`<header>`), secciones (`<section>`) y pie (`<footer>`). Sin texto añadido en pantalla.
- **La cabecera (1:41), Editor (JSFiddle), sin lámina:** JSFiddle con los paneles vacíos. Se escribe `<main class="perfil">` y, adentro, `<header>` con `<img class="foto">`, `<h1>Alex</h1>` y un `<p>`. Se pulsa Ejecutar. Texto en pantalla: «`main` = lo principal de la página» · «`header` = la cabecera» · «Etiquetas semánticas = con significado». Anotación: subrayar `class="foto"` y `class="perfil"`.
- **Secciones y pie de página (3:11), Editor (JSFiddle), sin lámina:** Entre `</header>` y `</main>` se escriben tres `<section>`: «Sobre mí» (con `<p>`), «Mis pasatiempos» (con `<ul>` de tres `<li>` con emojis) y «Mi mascota» (con `<img class="mascota">`). Después, `<footer>` con el enlace a MDN y la frase «Hecho con HTML y CSS». Se pulsa Ejecutar. Texto en pantalla: «`section` = una sección con su título» · «`footer` = el pie de página».
- **Estilo general (4:54), Editor (JSFiddle), sin lámina:** Se pasa al panel CSS. Se escriben el comentario `/* 1. Estilo general de la página */` y la regla de `body` (tipo de letra, tamaño, color de fondo, color del texto, `margin: 0` y `padding: 24px`). Se pulsa Ejecutar. Texto en pantalla: «Primero, el estilo general» · «`body` = toda la página».
- **La caja y la tarjeta centrada (6:07), Lámina 29 y luego el editor (JSFiddle):** Lámina 29: un diagrama de la caja con contenido, espacio interno, borde y espacio externo. Después, en el editor, se escriben el comentario `/* 2. La tarjeta… */` y `.perfil` con `max-width: 560px;` y `margin: 0 auto;`. Prueba rápida: sin `max-width` el centrado no se nota, y se recupera con `Ctrl + Z`. Luego se agregan `padding: 24px;`, `background-color: #ffffff;`, `border: 4px solid #0f766e;`, `border-radius: 20px;` y `text-align: center;`, y se pulsa Ejecutar. Texto en pantalla (solo durante el editor): «`max-width` = ancho máximo» · «Sin `max-width`, la tarjeta ocupa todo el ancho». Anotación: señalar el ancho máximo.
- **Imágenes redondas (8:13), Editor (JSFiddle), sin lámina:** Se escriben el comentario `/* 3. Las imágenes redondas… */`, `.foto, .mascota { border: 4px solid #0f766e; border-radius: 50%; object-fit: cover; }`, y después `.foto { width: 160px; height: 160px; }` y `.mascota { width: 120px; height: 120px; }`. Se pulsa Ejecutar: las imágenes quedan redondas. Prueba rápida con `border-radius: 20px` y vuelta a `50%`. Texto en pantalla: «Una coma = el mismo estilo para dos clases» · «`border-radius: 50%` = círculo».
- **Los detalles (9:33), Editor (JSFiddle), sin lámina:** Se escriben el comentario `/* 4. Títulos y lista */` con las reglas de `h1`, `h2`, `ul` (`list-style: none; padding: 0;`) y `li`, y el comentario `/* 5. Pie de página */` con las de `footer` y `a`. Se pulsa Ejecutar. Prueba rápida de contraste: el pie en gris muy claro y vuelta al gris oscuro. Texto en pantalla: «`rem` = medida según la letra de la página» · «`list-style: none` = sin viñetas» · «Revisa el contraste de tus colores».
- **Pantallas pequeñas (11:21), Editor (JSFiddle), sin lámina:** Se arrastra el borde izquierdo del panel Resultado hacia la derecha para hacerlo más angosto y simular una pantalla de celular; la tarjeta se adapta. Texto en pantalla: «Con `max-width`, la tarjeta se adapta a pantallas pequeñas».
- **Pausa y personaliza (11:57), Lámina 30:** Tarjeta de pausa de 5 segundos. Sin texto añadido en pantalla.
- **Guardar y compartir (12:31), Editor (JSFiddle), sin lámina:** JSFiddle: se muestra el botón Guardar (ícono de nube con flecha, a la derecha de Ejecutar), se pulsa y aparece el enlace nuevo en la barra de direcciones. Texto en pantalla: «Guardar y compartir» · «Copia tu HTML y tu CSS en un documento por si acaso».
- **Resumen (13:20), Lámina 31:** Lámina de resumen con cuatro tarjetas. Sin texto añadido en pantalla.

## 4. Pregunta para pensar

Si cambias `border-radius: 50%` por `border-radius: 0` en `.foto`, ¿qué forma toma la imagen?
