# Yellow Flowers

Animación CSS de flores amarillas con un mensaje especial. Proyecto 100% estático (HTML, CSS y un poco de JS) pensado para abrirse directamente en el navegador o desplegarse en GitHub Pages.

**Demo local:** abre `index.html` en tu navegador favorito.

## Contenido

- `index.html`: estructura del DOM y el mensaje visible.
- `styles.css`: todas las animaciones y estilos (flores, pasto, luces, mensaje). No usa librerías externas.
- `script.js`: lógica mínima para controlar el estado de pausa/arranque de las animaciones.
- `LICENSE`: licencia del proyecto.

## Requisitos

- Navegador moderno (Chrome, Edge, Firefox, Safari). No hay dependencias ni build.

## Ejecutar localmente

Opción rápida:

1. Haz doble clic en `index.html` o ábrelo desde tu navegador.

Opción recomendada (servidor local) con VS Code:

- Instala la extensión "Live Server" y ejecuta "Open with Live Server" sobre `index.html` para autorecarga.

## Personalización

- Texto del mensaje: edítalo en `index.html` dentro del elemento con clase `message`.
- Aparición del mensaje: en `styles.css`, la regla `.message` usa `animation-delay` (por defecto 2s) y `@keyframes fadeIn` para el efecto.
- Colores y fondo: ajusta variables en `:root` (por ejemplo `--dark-color`) y los `linear-gradient` de pétalos/hojas (`#fce700` para el amarillo).
- Velocidad de floración/hojas: cambia `--fl-speed` definida en `.flower` y los `animation-duration`/`delay` asociados.
- Pausar/arrancar animaciones: si añades `class="container"` al `<body>`, todas las animaciones quedan en pausa (ver selector `.container *` en `styles.css`). `script.js` elimina esa clase al cargar la página para iniciarlas automáticamente.

## Despliegue en GitHub Pages

1. Sube este repositorio a tu cuenta de GitHub (si no lo has hecho).
2. En GitHub, ve a Settings > Pages.
3. En "Build and deployment", selecciona:
   - Source: `Deploy from a branch`.
   - Branch: `main` y carpeta `/ (root)`.
4. Guarda. GitHub generará una URL pública en unos minutos.

## Notas y buenas prácticas

- El proyecto usa muchas animaciones CSS; equipos muy antiguos podrían ver menos fluidez.
- Mantén el contraste del mensaje para accesibilidad (texto oscuro sobre fondo amarillo brillante funciona bien).
- Si capturas pantalla o GIF, hazlo tras ~3–5s para que las animaciones estén visibles.

## Licencia

Consulta el archivo `LICENSE` incluido en el repositorio.
