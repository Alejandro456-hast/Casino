# 🎰 Juego de Ruleta en JavaScript

Un juego de ruleta de casino completamente funcional y responsivo, desarrollado utilizando tecnologías web estándar (Vanilla JavaScript, HTML5 y CSS3). Este proyecto simula la experiencia real de una mesa de ruleta, permitiendo realizar apuestas, girar la ruleta con animaciones y calcular automáticamente las ganancias y pérdidas.

## ✨ Características Principales

* **Tablero de Apuestas Interactivo:** Soporta apuestas internas (pleno, caballo, calle, cuadro, etc.) y externas (docenas, rojo/negro, par/impar, mayor/menor).
* **Sistema de Fichas (Chips):** Interfaz para seleccionar el valor de la apuesta (1, 5, 10, 100) y visualizar las fichas apiladas dinámicamente en el tablero.
* **Animaciones CSS:** La rueda de la ruleta y la bola giran utilizando animaciones fluidas basadas en `@keyframes`.
* **Cálculo de Pagos Automático:** El sistema evalúa instantáneamente el número ganador, multiplica las cuotas según el tipo de apuesta y actualiza el saldo (Bank) del jugador.
* **Interfaz en Español:** Todos los textos, notificaciones y elementos del tablero están completamente localizados al español.

## 🛠️ Tecnologías Utilizadas

* **HTML5:** Estructura semántica del juego y el tablero.
* **CSS3:** Estilos del casino, diseño de la ruleta basada en formas geométricas y animaciones.
* **JavaScript (ES6+):** Lógica principal del juego, manejo de arrays, eventos del DOM y cálculo de probabilidades.

## 🚀 Mejoras y Correcciones Recientes

Este proyecto ha sido refactorizado para garantizar mejores prácticas de desarrollo y corregir errores visuales de la versión original:

1. **Refactorización del Scope en JS:** Se eliminaron las variables globales implícitas en los bucles (`var`). Se implementó el uso de `let` y `const` junto con `'use strict'` para prevenir colisiones de memoria en los eventos de clic de las apuestas.
2. **Corrección de Alineación de Fichas (CSS):** Se solucionó un error visual donde las fichas se desfasaban de su posición al hacer clic. Ahora utilizan un centrado matemático absoluto (`transform: translate(-50%, -50%)`) que garantiza precisión sin importar el tamaño de la pantalla.
3. **Optimización del DOM:** La función de limpieza de fichas (`removeChips()`) fue reescrita utilizando selectores modernos (`querySelectorAll().forEach`) en lugar de depender de recursividad ineficiente.
4. **Traducción Integral:** Adaptación lógica y visual de términos en inglés a español, garantizando que el motor de validación reconozca correctamente cadenas como "ROJO", "NEGRO" y "2 a 1".
5. **Estructura HTML Válida:** Inclusión de etiquetas fundamentales como `<html>`, `lang="es"` y `<meta name="viewport">` para asegurar el correcto renderizado y escalado.

## 🎮 Cómo Jugar (Instalación Local)

No se requieren dependencias, empaquetadores (como Vite o Webpack) ni bases de datos. Para ejecutar el juego localmente:

1. Clona este repositorio:
   ```bash
   git clone [https://github.com/Alejandro456-hast/Casino.git](https://github.com/Alejandro456-hast/Casino.git)