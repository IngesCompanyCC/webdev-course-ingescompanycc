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

> **(0:00 - 0:25) Bienvenida**  
> Hola, te doy la bienvenida. En este curso vas a crear tu propia página web, a tu ritmo y desde cero y sin instalar nada: solo necesitas un navegador. Empecemos por lo básico: ¿qué es, de verdad, un sitio web?
>
> **(0:25 - 1:10) Un sitio web**  
> Las páginas web están por todas partes: en tu colegio, en las tiendas, en los blogs y en los periódicos. Un sitio web es un conjunto de páginas conectadas entre sí por enlaces. Y cada página tiene su propia dirección, como esta que ves aquí arriba.
>
> **(1:10 - 2:10) Cómo llega una página a tu pantalla**  
> ¿Y cómo llega hasta tu pantalla? Cuando escribes una dirección o haces clic en un enlace, tu navegador envía una solicitud. La recibe un servidor: una computadora donde están guardados los archivos del sitio. El servidor responde enviando esos archivos, y tu navegador los interpreta y te muestra la página.
>
> **(2:10 - 3:10) HTML, CSS y el navegador**  
> Esos archivos están escritos en lenguajes. Hoy vas a conocer dos. HTML define el contenido y la estructura: qué hay en la página, como títulos, párrafos, imágenes y enlaces. CSS define la presentación: cómo se ve, con colores, letras y espacios. Y el navegador junta los dos: lee el HTML, le aplica el CSS y te muestra la página terminada.
>
> **(3:10 - 3:40) El editor en línea**  
> Veámoslo en la práctica. Esto es JSFiddle, un editor en línea: funciona desde el navegador y no hace falta instalar nada. Arriba a la izquierda escribes el HTML; a la derecha, el CSS; y abajo a la derecha, en Resultado, aparece la página. El panel de JavaScript no lo usamos en este curso. Cada vez que cambies algo, pulsa el botón naranja Ejecutar, arriba, o Control Enter, y el resultado se actualiza. Fíjate en el HTML: tiene un título, un subtítulo, dos párrafos, una lista y un enlace. Y en el CSS están los colores y la forma de las casillas.
>
> **(3:40 - 4:20) Una página sin CSS**  
> Mira qué pasa si borro todo el CSS y pulso Ejecutar. Es la misma página y tiene el mismo contenido, pero ahora se ve sencilla: letras negras sobre fondo blanco. Y si recupero el CSS con Control Z y pulso Ejecutar, vuelven los colores. HTML define el contenido y CSS, la presentación.
>
> **(4:20 - 4:55) Pausa y prueba**  
> Ahora te toca a ti. Pausa el video y abre el enlace de la descripción. Primero, borra el CSS, pulsa Ejecutar y observa qué cambia; luego recupéralo con Control Z. Después, un mini reto: en el HTML cambia el título por «Mi Club de Videojuegos» y, en el CSS, cambia el color del título, #facc15, por #f472b6. Pulsa Ejecutar y mira tu versión. No puedes dañar nada: el fiddle es solo para practicar. Cuando termines, sigue con el video.
>
> **(4:55 - 5:15) Solución del mini reto**  
> ¿Lo lograste? Así queda el mini reto. En el HTML cambié el título por «Mi Club de Videojuegos» y, en el CSS, el color del título por #f472b6. Pulso Ejecutar y ahí está: un título nuevo, en rosado. Si el tuyo se ve igual, ya hiciste tu primer cambio en el HTML y en el CSS.
>
> **(5:15 - 5:45) Resumen**  
> Hoy aprendiste tres cosas: un sitio web es un conjunto de páginas conectadas, HTML define el contenido y CSS define la presentación. En la próxima lección vas a escribir tu primera página en HTML. Nos vemos allá.

## 3. Sugerencias multimedia

- **Bienvenida (0:00), Lámina 1 (portada del curso) y Lámina 2:** Portada del curso y portada de la lección 1. Texto en pantalla: «Lección 1 · ¿Qué es un sitio web?»
- **Un sitio web (0:25), navegador, sin lámina:** Una página web cualquiera, sin nombres ni logos del equipo (por ejemplo, la portada de MDN Web Docs). No se muestra la página de YouTube, porque deja ver el nombre del canal. Acercamiento a la barra de direcciones. Anotación: círculo rojo sobre la dirección. Texto en pantalla: «Un sitio web = páginas conectadas».
- **Cómo llega una página a tu pantalla (1:10), Lámina 3:** Lámina con el ciclo de tres pasos: solicitud, respuesta y la página en pantalla. Al editar el video se puede resaltar cada paso cuando se nombra. Texto en pantalla (uno por paso): «1. El navegador envía una solicitud» · «2. El servidor responde con los archivos» · «3. El navegador interpreta el código».
- **HTML, CSS y el navegador (2:10), Lámina 4:** Lámina con tres columnas: HTML (contenido y estructura), CSS (colores, letras y espacios) y el navegador, que junta los dos. Texto en pantalla: «HTML = el contenido y la estructura» · «CSS = el estilo» · «El navegador junta HTML y CSS y muestra la página».
- **El editor en línea (3:10), Editor (JSFiddle), sin lámina:** JSFiddle con el fiddle de inicio abierto; no se escribe nada. Se ven los paneles HTML (arriba a la izquierda), CSS (arriba a la derecha), JavaScript (abajo a la izquierda) y Resultado (abajo a la derecha), y el botón naranja Ejecutar en la barra de arriba. Anotación: flechas que señalan «HTML», «CSS», «Resultado» y el botón «Ejecutar». Texto en pantalla: «JSFiddle: un editor en línea y gratuito» · «Ejecutar = ver el resultado».
- **Una página sin CSS (3:40), Editor (JSFiddle), sin lámina:** Se hace clic en el panel CSS, `Ctrl + A` para seleccionar todo, se borra y se pulsa Ejecutar. El resultado cambia a una página sin estilo. Luego `Ctrl + Z` recupera el CSS y se pulsa Ejecutar otra vez. Anotación: resaltar «antes» y «después». Texto en pantalla: «Mismo contenido, sin CSS».
- **Pausa y prueba (4:20), Lámina 5:** Tarjeta de pausa de 5 segundos con cuenta regresiva. Texto en pantalla: «Pausa y prueba» · «Tómate el tiempo que necesites» · «Abre el enlace de la descripción» · «Borra el CSS y recupéralo con Ctrl + Z» · «Mini reto: cambia el título y su color».
- **Solución del mini reto (4:55), Editor (JSFiddle), sin lámina:** En el panel HTML, el título pasa a `<h1>Mi Club de Videojuegos</h1>`; en el panel CSS, dentro de `h1`, `#facc15` pasa a `#f472b6`. Se pulsa Ejecutar: el título cambia de texto y queda rosado. Texto en pantalla: «Así queda el mini reto». Anotación: resaltar los dos cambios.
- **Resumen (5:15), Lámina 6:** Lámina de resumen con tres puntos. Texto en pantalla: «Sitio web: páginas conectadas por enlaces» · «HTML: define el contenido y la estructura» · «CSS: define la presentación de la página».

## 4. Pregunta para pensar

Si una página se ve bien pero sus letras no se leen, ¿el problema está en el HTML o en el CSS?
