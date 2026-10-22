# Analizador de vigas

Calculadora web de vigas con cargas escritas con letras (W, P, M) y posiciones en función de L (L/3, 2L/3, 0.25L). Entrega momentos, reacciones y ecuaciones exactas en fracciones, como en la tabla SIMESA, y admite apoyos configurables, apoyos intermedios y articulaciones internas.

**Abrir la app:** https://mmedinamu-create.github.io/analizador-vigas/

## Funciones

- **Cargas con letras:** puntual, uniforme, triangular (con el máximo en cualquier punto), trapezoidal, parabólica, complemento de parábola, parabólica con pico y momento concentrado. Magnitudes como `W`, `2W`, `3W/2`, `P`, `M` o números.
- **Resultados exactos:** momentos en los apoyos, momento máximo positivo y negativo con su ubicación, reacciones, V y M en puntos clave y ecuaciones V(x) y M(x) por tramo, todo en fracciones (por ejemplo −WL²/12 o 8PL/81).
- **Apoyos:** empotramiento, articulado, rodillo, empotramiento guiado o libre en los extremos A y B, más apoyos intermedios.
- **Articulaciones internas (rótulas):** el momento flector es cero en ellas.
- **Clasificación:** grado de indeterminación GI = r − 3 − c y detección de mecanismos.
- **Valores numéricos opcionales:** con L y el valor de cada letra, también entrega resultados en unidades (kN, tf, kgf, N, kip, lb; m, cm, ft, in).
- **Casos de referencia:** casos de la tabla SIMESA y ejemplos de vigas Gerber, continuas y con voladizo.

## Modelo

Viga de Euler-Bernoulli con EI constante, resuelta por el método de rigidez con aritmética racional exacta. Las fuerzas internas se obtienen por equilibrio a partir de las reacciones, y la verificación (ΣFy = 0, ΣMA = 0 y M = 0 en cada articulación) también es exacta.

Convenciones: x se mide desde A; P y W son positivas hacia abajo; el momento flector es positivo cuando tracciona la fibra inferior, así que los momentos de empotramiento salen negativos, como en la tabla.

## Uso local

Es un único archivo, `index.html`, sin dependencias. Basta con abrirlo en el navegador.
