# UNAD_CD

Repositorio de actividades de Cálculo Diferencial desarrolladas en Google Colab.

## Descripción

Este proyecto incluye una notebook que grafica una función a trozos y destaca visualmente los puntos abiertos y cerrados en los cambios de definición.

## Notebook incluido

- `Gráfica_Función_A_Trozos_Ejercicio_5_Reto_3.ipynb`

### Función representada

La gráfica corresponde a una función definida en tres tramos:

- `f(x) = 2x + 4`, si `x < 1`
- `f(x) = x² + 2`, si `1 ≤ x < 3`
- `f(x) = x + 8`, si `x ≥ 3`

La notebook:

- genera los valores de `x` para cada intervalo,
- calcula los valores de `y` correspondientes,
- dibuja cada rama con colores distintos,
- marca los puntos abiertos y cerrados en `x = 1` y `x = 3`,
- añade ejes, cuadrícula y leyenda para facilitar la interpretación.

## Requisitos

Para ejecutar esta notebook se necesita:

- Python 3
- NumPy
- Matplotlib

## Ejecución

Puedes abrir la notebook directamente en Google Colab o ejecutar el archivo en un entorno Jupyter con estas librerías instaladas:

```bash
pip install numpy matplotlib
```

Luego ejecuta la notebook en orden para visualizar la gráfica.

## Objetivo académico

Esta actividad permite analizar la continuidad de una función a trozos, identificar intervalos de definición y reconocer la diferencia entre puntos abiertos y cerrados en la gráfica.
