# 🇲🇽 Taco Tetris Fiesta 🌮🎮

¡Bienvenido a **Taco Tetris Fiesta**! Un videojuego web interactivo desarrollado en **HTML5 Canvas**, **CSS3** y **JavaScript Vanilla** (sin librerías externas). Reemplaza los bloques tradicionales de Tetris por elementos icónicos de la cultura mexicana: tacos, sombreros, banderas, mariachis, piñatas, chiles y cactus.

![Taco Tetris Fiesta Banner](banner.png)

---

## 🚀 Características Principales

* **🎨 Gráficos Personalizables:** Piezas dibujadas dinámicamente utilizando imágenes (`<img>`) o vectores SVG de alta definición integrados en el código.
* **🎆 Efectos Visuales y Sonoros:** Sistema de fuegos artificiales al avanzar de nivel/ganar y reproductor `<audio>` nativo con música festiva y sintetizador de efectos sonoros en tiempo real.
* **🌌 Fondo de Video Dinámico:** Estructura preparada para colocar tu propio video de fondo (`video.mp4` / `video.webm`).
* **🕹️ Soporte para Mandos (Gamepad API):** Compatible con controles inalámbricos (Bluetooth) y alámbricos (Xbox, PlayStation, etc.).
* **📱 Multi-Dispositivo y Responsivo:** Diseñado con gestos táctiles (*swipes*) para pantallas de Celulares, iPads, Tablets, MacBooks y Computadoras de escritorio.
* **💥 Física de Gravedad en Cascada:** Al eliminar líneas, los bloques suspendidos caen automáticamente al fondo, generando reacciones en cadena y combos de puntos extra.
* **🏆 Sistema de 10 Niveles:** Progresión configurable con meta total de 200 puntos.

---

## 🛠️ Tecnologías Utilizadas

* **HTML5:** Estructura semántica, Canvas para el renderizado del juego y etiquetas `<video>` / `<audio>` nativas.
* **CSS3:** Flexbox, animaciones de luces de neón, transparencia glassmorphism y diseño responsive con Media Queries.
* **JavaScript (ES6+):** Programación orientada a objetos (POO), lógica del bucle de juego (*Game Loop*), síntesis de audio Web Audio API, Gamepad API y listeners de eventos táctiles/teclado.

---

## 🕹️ Controles

| Dispositivo | Acción | Control / Gesto |
| :--- | :--- | :--- |
| **Teclado (PC / Mac)** | Mover Izquierda / Derecha | Flechas `←` `→` o Teclas `A` `D` |
| | Rotar Pieza | Flecha `↑` o Tecla `W` |
| | Bajar Más Rápido | Flecha `↓` o Tecla `S` |
| | Caída Instantánea (Hard Drop) | Barra Espaciadora (`Space`) |
| **Pantalla Táctil (Móvil / Tablet)** | Mover | Deslizar dedo a la Izquierda / Derecha |
| | Rotar | Deslizar dedo hacia Arriba |
| | Bajar Rápido | Deslizar dedo hacia Abajo |
| **Gamepad (Xbox / PS / Genérico)** | Mover / Caída | D-Pad (Cruceta) o Joycon Izquierdo |
| | Rotar | Botones Principales (`A` / `Cross`) |

---

## ⚙️ Personalización de Puntos y Niveles

Puedes ajustar la dificultad y la cantidad de puntos abriendo el archivo `TacoTetrisFiesta.html` y modificando el objeto `GAME_CONFIG` al inicio del script:

```javascript
const GAME_CONFIG = {
    TOTAL_LEVELS: 10,        // Cantidad total de niveles
    POINTS_PER_LEVEL: 20,    // Puntos necesarios para subir cada nivel
    POINTS_PER_LINE: 5,      // Puntos otorgados por cada línea destruida
    SPEED_DECREMENT: 70      // Milisegundos que se acelera la caída por nivel
};
