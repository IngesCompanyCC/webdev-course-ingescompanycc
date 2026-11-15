# Lección 1: ¿Qué es un sitio web?

_(Contenido para los instructores)_

**Objetivo:** Al terminar, el estudiante puede explicar con sus palabras qué es un sitio web, decir para qué sirven HTML y CSS, ver en un editor en línea la diferencia entre una página con estilo y una sin estilo, y hacer su primer cambio en el HTML y en el CSS.

**Palabras nuevas:** sitio web, página web, navegador, dirección, solicitud, servidor, HTML, CSS, editor en línea.

## 1. Estructura de carpetas (GitHub)

```text
/starter-files/leccion-01        # Código de inicio de la lección
├── index.html
└── styles.css

/completed-examples/leccion-01   # Código completo de la lección
├── index.html
└── styles.css
```

## 2. Guion del video (5 minutos)

> Los tiempos son los del audio (unos 4:11). Con las tarjetas de pausa, los Ejecutar y las transiciones de la edición, el video llega a unos 5 minutos. El guion detallado para grabar está en `grabacion/leccion-01.md` (solo para el equipo).

> **(0:00 - 0:25) Bienvenida**  
> ¡Hola! Te doy la bienvenida al curso Fundamentos de Desarrollo Web. Aquí vas a crear tu propia página web, a tu ritmo, desde cero y sin instalar nada: solo necesitas un navegador. Empecemos por lo básico: ¿qué es, de verdad, un sitio web?
>
> **(0:25 - 0:55) Un sitio web**  
> Las páginas web están por todas partes: la de tu colegio, la tienda donde miras zapatillas o la de tu videojuego favorito. Un sitio web es un conjunto de páginas conectadas por enlaces: haces clic en uno y saltas a otra página. Y cada página tiene su propia dirección, como esta de aquí arriba.
>
> **(0:55 - 1:20) Cómo llega una página a tu pantalla**  
> ¿Y cómo llega hasta tu pantalla? Cuando abres una dirección, tu navegador envía una solicitud. La recibe un servidor: una computadora donde están guardados los archivos del sitio. El servidor responde enviando esos archivos, y tu navegador los interpreta y te muestra la página.
>
> **(1:20 - 1:54) HTML, CSS y el navegador**  
> Esos archivos están escritos en lenguajes, y hoy conoces dos. HTML define el contenido y la estructura: títulos, párrafos, imágenes y enlaces. CSS define la presentación: colores, letras y espacios. Piensa en una casa: HTML son las paredes y los cuartos; CSS, la pintura y la decoración. Y el navegador junta los dos y te muestra la página terminada.
>
> **(1:54 - 2:22) El editor en línea**  
> Veámoslo en la práctica. Esto es JSFiddle, un editor en línea y gratuito. Arriba a la izquierda va el HTML; a la derecha, el CSS; y abajo a la derecha, en Resultado, aparece la página. El panel de JavaScript no lo usamos. Cuando cambies algo, pulsa Ejecutar o Control Enter.
>
> **(2:22 - 2:47) Una página sin CSS**  
> Ahora, un experimento. Borro todo el CSS y pulso Ejecutar. ¡Mira! Es la misma página, con el mismo contenido, pero ahora se ve sencilla: letras negras sobre fondo blanco. Recupero el CSS con Control Z y pulso Ejecutar. ¡Vuelven los colores!
>
> **(2:47 - 3:17) Pausa y prueba**  
> ¡Te toca! Pausa el video y abre el enlace de la descripción. Borra el CSS, pulsa Ejecutar y recupéralo con Control Z. Y un mini reto: cambia el título por Mi Club de Videojuegos y su color por numeral f 4 7 2 b 6. Cuando termines, sigue con el video.
>
> **(3:17 - 3:52) Solución del mini reto**  
> ¿Lo lograste? En el HTML agrego Mi antes del título y, en el CSS, dentro de h1, cambio el color por numeral f 4 7 2 b 6. Ejecutar. ¡Un título nuevo, en rosado! Si el tuyo se ve igual, ya hiciste tu primer cambio en HTML y en CSS.
>
> **(3:52 - 4:11) Resumen**  
> Hoy aprendiste tres cosas: un sitio web es un conjunto de páginas conectadas, HTML define el contenido y CSS, la presentación. En la próxima lección escribes tu primera página en HTML. ¡Nos vemos ahí!

## 3. Sugerencias multimedia

- **Bienvenida (0:00), Lámina 1 (portada del curso) y Lámina 2:** Portada del curso y portada de la lección 1. Sin texto añadido en pantalla.
- **Un sitio web (0:25), navegador, sin lámina:** Una página web sin nombres ni logos del equipo (la portada de MDN Web Docs). Se hace clic en un enlace del menú y se acerca la barra de direcciones. No se muestra YouTube, porque deja ver el nombre del canal. Anotación: círculo naranja sobre la barra de direcciones. Texto en pantalla, en una franja abajo: «Un sitio web = páginas conectadas».
- **Cómo llega una página a tu pantalla (0:55), Lámina 3:** Lámina con el ciclo de tres pasos: solicitud, respuesta y la página en pantalla; se resalta cada paso cuando se nombra. Sin texto añadido en pantalla.
- **HTML, CSS y el navegador (1:20), Lámina 4:** Lámina con tres columnas: HTML (contenido y estructura), CSS (colores, letras y espacios) y el navegador, que junta los dos. Sin texto añadido en pantalla.
- **El editor en línea (1:54), Editor (JSFiddle), sin lámina:** JSFiddle con el fiddle de inicio; no se escribe nada. Se señalan los paneles HTML, CSS, JavaScript y Resultado, y el botón Ejecutar. Anotación: flechas a «HTML», «CSS», «Resultado» y «Ejecutar». Texto en pantalla: «JSFiddle: un editor en línea y gratuito» · «Ejecutar = ver el resultado».
- **Una página sin CSS (2:22), Editor (JSFiddle), sin lámina:** Se selecciona todo el panel CSS con `Ctrl + A`, se borra y se pulsa Ejecutar: la página queda sin estilo. Luego `Ctrl + Z` recupera el CSS y se pulsa Ejecutar otra vez. Anotación: resaltar «antes» y «después». Texto en pantalla: «Mismo contenido, sin CSS».
- **Pausa y prueba (2:47), Lámina 5:** Tarjeta de pausa de 5 segundos. Sin texto añadido en pantalla.
- **Solución del mini reto (3:17), Editor (JSFiddle), sin lámina:** En el panel HTML el título pasa a `<h1>Mi Club de Videojuegos</h1>`; en el panel CSS, dentro de `h1`, `#facc15` pasa a `#f472b6`. Se pulsa Ejecutar: el título cambia de texto y queda rosado. Texto en pantalla: «Así queda el mini reto». Anotación: resaltar los dos cambios.
- **Resumen (3:52), Lámina 6:** Lámina de resumen con tres puntos. Sin texto añadido en pantalla.

## 4. Pregunta para pensar

Si una página se ve bien pero sus letras no se leen, ¿el problema está en el HTML o en el CSS?
