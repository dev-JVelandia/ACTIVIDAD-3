# Hoja de vida web · Juan Diego Velandia Guerrero

Sitio personal responsive con mi hoja de vida, mis proyectos de clase y una versión mejorada del sitio de una piñatería. Está hecho con HTML y CSS (Grid, Mobile First y media queries) y publicado con GitHub Pages.

**Sitio publicado:** [https://github.com/dev-JVelandia/ACTIVIDAD-3.git](https://dev-jvelandia.github.io/hoja-de-vida/)


## Páginas

- `index.html`: hoja de vida (perfil, formación, habilidades, competencias, idiomas y contacto).
- `proyectos.html`: tres proyectos de clase, cada uno con su explicación y el enlace a su repositorio de GitHub.
- `piñateria2.0/piñateria 2.0.html`: la piñatería mejorada (productos, información, opiniones y ubicación), adaptada de un ejercicio de clase.

Las tres páginas se enlazan entre sí desde el menú de navegación.

## Mockups

Cada página tiene un mockup para celular y otro para computador, con las áreas marcadas y los nombres que uso en `grid-template-areas`.

### Hoja de vida

Áreas: `cabecera`, `menu`, `perfil`, `formacion`, `habilidades`, `competencias`, `contacto`.

![Inicio en celular](/mackups/hoja-de-vida-celular.png)
![Inicio en computador](/mackups/hoja-de-vida-escritorio.png)

### Proyectos

Áreas: `cabecera`, `menu`, `intro`, `proyectos`, `contacto`.

![Proyectos en celular](/mackups/proyectos-celular.png)
![Proyectos en computador](/mackups/proyetos-escritorio.png)



## Capturas del sitio publicado

Capturas del sitio ya publicado, en dos dispositivos:

![Celular](capturas/celular.png)
![Computador](capturas/computador.png)



## Breakpoints

El CSS de la hoja de vida y de proyectos (`styles.css`) está hecho **Mobile First**: los estilos base son para celular y las `@media (min-width: ...)` van al final, de menor a mayor.

**Base (celular, menos de 600px):**
- El menú es una columna fija a la izquierda (`position: sticky`) que siempre se ve al desplazarse.
- El contenido va en una sola columna, con las secciones apiladas y separadas por un espacio gris.
- La cabecera muestra la foto a la izquierda y el nombre y el cargo centrados.

**Desde 600px:**
- El menú lateral se ensancha.
- El grid pasa a varias columnas: perfil y formación ocupan todo el ancho, y habilidades y competencias quedan lado a lado.
- La cabecera crece: la foto y el título se agrandan.

**Desde 1024px:**
- El menú vuelve a ser una barra horizontal debajo de la cabecera.
- El grid pasa a dos columnas (2fr y 1fr): perfil junto a habilidades, formación junto a competencias, y el contacto abajo.
- En la página de proyectos, las tarjetas se acomodan en fila (`repeat(auto-fit, minmax(16rem, 1fr))`).

**Piñatería 2.0:** usa su propio CSS, que parte del escritorio y tiene un breakpoint de `max-width: 480px`, donde el menú se apila en vertical, los títulos y el banner se reducen y la tabla achica la letra.

## Cómo lo publiqué



1. Cómo creé el repositorio público: Lo primero que hice fue buscar maneras de publicar las paginas y encontre la   
   pagina  Vercel.
2. Cómo subí mis archivos (desde la web de GitHub o con Git):solo vinvule mi cuenta de github a la pagina vercel y subi la carpeta donde estan los archivos de la actividad
3. Dónde activé GitHub Pages y qué rama y carpeta elegí: no use esta opcion
4. Cuánto tardó en aparecer el sitio: poco tiempo la verdad
5. Por qué la página principal debe llamarse `index.html`: esto es para que a la hora de subirlo se detecte de manera automatica como el principal o el padre.
6. Qué errores encontré al publicar y cómo los arreglé: Bastantes errores con las imagenes y actualizaciones en el codigo y se solucionaron organizando bien las carpetas y subiendo cada modificacion a github

## Fuentes consultadas

-google gemini
-claude IA

