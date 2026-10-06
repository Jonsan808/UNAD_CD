# Gráfica de una función a trozos - Ejercicio 5, Reto 3

Este proyecto presenta una gráfica de una función definida por partes, también llamada función a trozos. La idea principal es visualizar cómo cambia la expresión matemática según el valor de `x`.

Puedes abrir el notebook directamente aquí:

https://github.com/Jonsan808/UNAD_CD/blob/main/Gr%C3%A1fica_Funci%C3%B3n_A_Trozos_Ejercicio_5_Reto_3.ipynb

## ¿Qué hace este código?

El código genera una gráfica de la siguiente función:

```python
f(x) = {
    2x + 4,    si x < 1
    x² + 2,    si 1 ≤ x < 3
    x + 8,     si x ≥ 3
}
```

Es decir, la función cambia de fórmula dependiendo del intervalo en el que esté `x`.

## ¿Por qué es importante?

Las funciones a trozos son muy útiles en matemáticas y en aplicaciones reales porque permiten modelar situaciones donde el comportamiento cambia según ciertas condiciones. Por ejemplo:

- Tarifas según consumo
- Impuestos por rangos
- Precios por tramo de distancia
- Modelos físicos con distintas reglas en intervalos distintos

## Librerías que se usan

Este notebook utiliza:

- `numpy`: para crear valores de `x` y hacer cálculos numéricos
- `matplotlib`: para dibujar la gráfica

## Cómo está estructurado el código

### 1. Importación de librerías
```python
import numpy as np
import matplotlib.pyplot as plt
```

### 2. Definición de cada tramo
Se crean tres arreglos de valores para `x`:

```python
x1 = np.linspace(-2, 1, 300, endpoint=False)
x2 = np.linspace(1, 3, 300, endpoint=False)
x3 = np.linspace(3, 6, 300)
```

Cada tramo representa uno de los intervalos de la función.

### 3. Cálculo de los valores de `y`
```python
y1 = 2 * x1 + 4
y2 = x2**2 + 2
y3 = x3 + 8
```

### 4. Graficación de cada tramo
```python
plt.plot(x1, y1, label="2x + 4, si x < 1", color="red")
plt.plot(x2, y2, label="x² + 2, si 1 ≤ x < 3", color="blue")
plt.plot(x3, y3, label="x + 8, si x ≥ 3", color="green")
```

### 5. Puntos abiertos y cerrados
El código marca los puntos de cambio con distintos estilos para mostrar si el valor pertenece o no al intervalo:

```python
plt.scatter(1, 6, facecolors="white", edgecolors="black", s=100)
plt.scatter(1, 3, color="black", s=80)
plt.scatter(3, 11, facecolors="white", edgecolors="black", s=100)
plt.scatter(3, 11, color="black", s=50)
```

Esto ayuda a interpretar la continuidad y la exclusión de puntos en los intervalos.

### 6. Personalización del gráfico
Se agregan:

- título
- ejes
- cuadrícula
- leyenda
- límites del eje x y y
- líneas de referencia para los ejes cartesianos

```python
plt.title("Continuidad de una función a trozos")
plt.xlabel("x")
plt.ylabel("f(x)")
plt.xlim(-2, 6)
plt.ylim(-1, 15)
plt.grid(True)
plt.legend()
plt.show()
```

## Resultado esperado

La gráfica muestra claramente:

- un primer tramo lineal en rojo
- un segundo tramo cuadrático en azul
- un tercer tramo lineal en verde
- puntos abiertos y cerrados donde cambia la definición de la función

## Requisitos para ejecutar el notebook

Necesitas tener instalado Python y las siguientes librerías:

```bash
pip install numpy matplotlib
```

## En resumen

Este ejercicio sirve para entender cómo se representan funciones definidas por partes y cómo se interpreta visualmente su continuidad, dominio y comportamiento en distintos intervalos.

Es una excelente práctica para reforzar conceptos de cálculo y de gráficas en el plano cartesiano.

---

Proyecto desarrollado para apoyo académico en el curso de cálculo diferencial de la UNAD.
