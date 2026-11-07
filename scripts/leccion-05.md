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

> **(0:00 - 0:45) El resultado**  
> Llegó el momento de juntar todo lo que aprendiste. En esta lección vamos a construir una página de perfil completa: con tu foto, tus datos, tus pasatiempos y mucho estilo. Esto que ves es el resultado, y al final va a ser tuyo.
>
> **(0:45 - 2:00) El boceto**  
> Antes de escribir código, quienes hacen páginas web dibujan un boceto. Aquí tenemos: arriba, la foto y el nombre; en el medio, varias secciones; y abajo, un pie con un enlace. Y recuerda: usa un apodo y no pongas datos privados.
>
> **(2:00 - 3:45) La cabecera**  
> Empecemos por la estructura. Primero, una etiqueta main, que envuelve el contenido principal. Adentro, un header, que es la cabecera: ahí van la foto, tu nombre y una frase corta sobre ti. Fíjate que estas etiquetas no cambian cómo se ve la página, pero le dan un significado: le dicen al navegador, y a quienes usan lectores de pantalla, qué es cada parte.
>
> **(3:45 - 6:15) Secciones y pie de página**  
> Ahora, las secciones. Cada `section` tiene su título h2 y su contenido: un párrafo, una lista, una imagen. Al final, un `footer`, que es el pie de la página, con un enlace. Mira cómo todo lo que aprendiste está aquí: títulos, párrafos, listas, imágenes y enlaces. Todavía se ve sencilla, pero el contenido ya está completo.
>
> **(6:15 - 7:30) Estilo general**  
> Ahora le toca al CSS. Empezamos por el estilo general en body: el tipo de letra, el tamaño, un fondo azul claro y un color de texto oscuro. También quito el margen que el navegador pone por defecto y agrego espacio interno de 24 píxeles para que el contenido no quede pegado al borde.
>
> **(7:30 - 10:00) La caja y la tarjeta centrada**  
> En CSS, cada elemento se representa como una caja: es el modelo de caja. Adentro está el contenido; alrededor, el espacio interno, que se llama padding; luego el borde; y afuera, el espacio externo, que es el margen. Para nuestra tarjeta, le doy un ancho máximo de 560 píxeles. Para centrarla, uso `margin` con `0 auto`: el cero es para arriba y abajo, y `auto` hace que los lados se repartan por igual. Fíjate: si le quito el ancho máximo, la tarjeta ocupa todo el ancho y no se nota el centrado. Después agrego fondo blanco, un borde de 4 píxeles, esquinas redondeadas y el texto centrado.
>
> **(10:00 - 11:30) Imágenes redondas**  
> Para que las imágenes sean redondas, uso un truco: `border-radius` igual a 50 por ciento. Y como las dos imágenes comparten el mismo estilo, las escribo juntas, separadas por una coma. Después le doy a cada una su propio tamaño. `object-fit: cover` evita que la imagen se deforme.
>
> **(11:30 - 12:45) Los detalles**  
> Ahora los detalles. Pinto los títulos con el verde azulado de la paleta. El tamaño de los subtítulos lo escribo en `rem`, una medida que depende del tamaño de letra general de la página: 1.3 rem significa un poco más grande que el texto normal. En la lista, quito las viñetas con `list-style` igual a `none` y el espacio interno que trae por defecto, para que quede centrada. Y al pie le doy un texto más pequeño y un color gris oscuro. Cuida siempre el contraste: el texto tiene que poder leerse con facilidad.
>
> **(12:45 - 13:05) Pantallas pequeñas**  
> Un detalle bonito: si achico la ventana, como pasaría en un celular, la tarjeta se adapta sola. Eso pasa gracias al ancho máximo que le pusimos.
>
> **(13:05 - 13:30) Pausa y personaliza**  
> Ahora es tu turno. Pausa el video y arma tu propia página de perfil. Cambia los colores, escribe tus propios pasatiempos y agrega las secciones que quieras. Recuerda: usa un apodo y nada de datos privados. Cuando termines, vuelve para ver cómo guardarla.
>
> **(13:30 - 14:30) Guardar y compartir**  
> Para guardar tu página en JSFiddle, pulsa Guardar, el ícono de la nube con una flecha, al lado de Ejecutar: arriba, en la barra de direcciones, aparece un enlace nuevo con tu versión. Si el editor te pide crear una cuenta y no puedes o no quieres crearla, copia tu HTML y tu CSS en un documento y guárdalo. Algunos sitios piden una edad mínima para crear una cuenta. También puedes compartir el enlace de tu página con tu familia y tus amistades.
>
> **(14:30 - 15:00) Resumen**  
> Hoy construiste una página de perfil completa. Usaste etiquetas semánticas, aprendiste el modelo de caja, y centraste, coloreaste y redondeaste. En la última lección vemos los errores más comunes y cómo encontrarlos. Nos vemos allá.

## 3. Sugerencias multimedia

- **El resultado (0:00), Lámina 27 (unos 3 s) y luego el resultado terminado:** La página de perfil terminada, a pantalla completa, con un pequeño recorrido del cursor. Texto en pantalla: «Lección 5 · Proyecto: tu página de perfil»
- **El boceto (0:45), Lámina 28:** Lámina con un boceto de la página: cajas para foto, nombre, secciones y pie. Texto en pantalla: «Primero se dibuja, después se programa». «Usa un apodo. Nada de datos privados.»
- **La cabecera (2:00), Editor (JSFiddle), sin lámina:** JSFiddle con los paneles vacíos. Se escribe `<main class="perfil">` y, adentro, `<header>` con `<img class="foto">`, `<h1>Alex</h1>` y un `<p>`. Texto en pantalla: «`main` = lo principal de la página» · «`header` = la cabecera». Anotación: subrayar `class="foto"`.
- **Secciones y pie de página (3:45), Editor (JSFiddle), sin lámina:** Se escriben tres `<section>`: «Sobre mí» (con `<p>`), «Mis pasatiempos» (con `<ul>` de tres `<li>` con emojis) y «Mi mascota» (con `<img class="mascota">`). Después, `<footer>` con el enlace a MDN y la frase «Hecho con HTML y CSS». Texto en pantalla: «`section` = una sección con su título» · «`footer` = el pie de página».
- **Estilo general (6:15), Editor (JSFiddle), sin lámina:** Se pasa al panel CSS. Se escribe la regla de `body` (tipo de letra, tamaño, color de fondo, color del texto, `margin: 0` y `padding: 24px`). Texto en pantalla: «Primero, el estilo general».
- **La caja y la tarjeta centrada (7:30), Lámina 29 y luego el editor (JSFiddle):** Lámina «la caja»: un diagrama con contenido, espacio interno, borde y espacio externo. Después, se escribe `.perfil` con `max-width: 560px;`, `margin: 0 auto;`, `padding: 24px;`, `background-color: #ffffff;`, `border: 4px solid #0f766e;`, `border-radius: 20px;`, `text-align: center;`. Se muestra qué pasa si se quita `max-width`: el centrado no se nota. Texto en pantalla: «Contenido → `padding` → `border` → `margin`». «`margin: 0 auto` centra la caja». Anotación: señalar el ancho máximo.
- **Imágenes redondas (10:00), Editor (JSFiddle), sin lámina:** Se escribe `.foto, .mascota { border: 4px solid #0f766e; border-radius: 50%; object-fit: cover; }`, y después `.foto { width: 160px; height: 160px; }` y `.mascota { width: 120px; height: 120px; }`. Las imágenes quedan redondas. Texto en pantalla: «Una coma = el mismo estilo para dos clases». «`border-radius: 50%` = círculo».
- **Los detalles (11:30), Editor (JSFiddle), sin lámina:** Se escriben las reglas de `h1`, `h2`, `ul` (`list-style: none; padding: 0;`), `li`, `footer` y `a`. Texto en pantalla: «`list-style: none` = sin viñetas». «Revisa el contraste de tus colores».
- **Pantallas pequeñas (12:45), Editor (JSFiddle), sin lámina:** Se arrastra el borde izquierdo del panel Resultado hacia la derecha para hacerlo más angosto y simular una pantalla de celular. La tarjeta se adapta. Texto en pantalla: «Con `max-width`, la tarjeta se adapta a pantallas pequeñas».
- **Pausa y personaliza (13:05), Lámina 30:** Tarjeta de pausa de 5 segundos con cuenta regresiva. Texto en pantalla: «Pausa el video y personaliza tu página» · «Tómate el tiempo que necesites»: «Cambia los colores, las secciones y los textos. Usa un apodo».
- **Guardar y compartir (13:30), Editor (JSFiddle), sin lámina:** JSFiddle: se muestra el botón Guardar (ícono de nube con flecha, a la derecha de Ejecutar) y el enlace nuevo que aparece en la barra de direcciones. Texto en pantalla: «Guardar y compartir». «Copia tu HTML y tu CSS en un documento por si acaso».
- **Resumen (14:30), Lámina 31:** Lámina de resumen. Texto en pantalla: «HTML = estructura» · «CSS = estilo» · «Modelo de caja: `padding`, `border`, `margin`».

## 4. Pregunta para pensar

Si cambias `border-radius: 50%` por `border-radius: 0` en `.foto`, ¿qué forma toma la imagen?
