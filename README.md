# Analizador de vigas

Calculadora web para vigas con apoyos configurables, articulaciones internas y cargas en cualquier posición. Calcula reacciones, diagramas de cortante V(x) y momento flector M(x), ecuaciones por tramo y verificación de equilibrio.

**Abrir la app:** https://mmedinamu-create.github.io/analizador-vigas/

## Funciones

- **Apoyos:** empotramiento, articulado, rodillo, empotramiento guiado o libre en los extremos A y B, más apoyos intermedios (rodillo o articulado).
- **Articulaciones internas (rótulas):** en cualquier posición; el momento flector es cero en ellas.
- **Cargas:** puntuales, distribuidas (uniformes, triangulares o trapezoidales, en toda la luz o en un tramo) y momentos puntuales horarios o antihorarios.
- **Clasificación:** grado de indeterminación GI = r − 3 − c y detección de mecanismos (inestabilidad geométrica).
- **Resultados:** reacciones, momentos y cortantes extremos con su ubicación, lectura de V y M en cualquier x, ecuaciones polinómicas por tramo y comprobación de ΣFy = 0, ΣMA = 0 y M = 0 en cada articulación.

## Modelo

Viga de Euler-Bernoulli con EI constante, resuelta por el método de rigidez. Las fuerzas internas se obtienen por equilibrio a partir de las reacciones. Unidades: kN y m.

Convenciones: x se mide desde A; P y w son positivas hacia abajo; el momento flector es positivo cuando tracciona la fibra inferior.

## Uso local

Es un único archivo, `index.html`, sin dependencias. Basta con abrirlo en el navegador.
