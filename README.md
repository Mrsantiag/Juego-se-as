# Aventura LSC – Lengua de Señas Colombiana

Dos secciones desde el menú principal (diseño claro y colorido):

- **Repaso:** muestra cada seña con su nombre. Tiene buscador y, al tocar una seña, se ve en grande.
- **Juego:** carrera de tablero para 1 a 4 jugadores. Cada turno se responden 1, 2 o 3 señas según la dificultad.

Las señas del juego salen como una baraja: ninguna se repite hasta que hayan salido todas.

## Estructura
```
index.html      -> el juego y el repaso
imagenes/       -> una imagen por seña (frijol.jpg, frio.jpg, ...)
```

## Publicar en GitHub Pages
1. Crea un repositorio y sube `index.html` y la carpeta `imagenes/`.
2. Ve a **Settings → Pages**.
3. En *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
4. Espera 1–2 minutos: quedará en `https://TU-USUARIO.github.io/NOMBRE-REPO/`.

## Agregar una seña nueva
1. Pon la imagen en `imagenes/` (ej. `arroz.jpg`).
2. En `index.html`, dentro de `questionsDatabase`, agrega una línea:
   `{ id: 23, word: "ARROZ", image: "imagenes/arroz.jpg" },`

Aparece sola en el repaso y en el juego.
