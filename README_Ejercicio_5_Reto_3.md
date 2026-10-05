# 📊 Gráfica de Función a Trozos - Ejercicio 5 Reto 3

## 🎯 ¿De qué se trata?

Este notebook muestra cómo **graficar una función definida en tres tramos diferentes**. Es decir, una función que tiene una ecuación distinta según el rango de valores de `x` en el que nos encontremos.

Es como si tuviéramos "tres reglas diferentes" dependiendo de dónde estemos: 
- Si estás aquí → usa esta fórmula
- Si estás allá → usa esta otra
- Si estás más allá → usa esta tercera

## 📐 La función del ejercicio

La función que graficamos es:

```
       ⎧ 2x + 4      si  x < 1
f(x) = ⎨ x² + 2      si  1 ≤ x < 3
       ⎩ x + 8       si  x ≥ 3
```

### Explicación de cada tramo:

| Tramo | Fórmula | Rango | Color |
|-------|---------|-------|-------|
| 1️⃣ **Línea recta** | `2x + 4` | x < 1 | 🔴 Rojo |
| 2️⃣ **Parábola** | `x² + 2` | 1 ≤ x < 3 | 🔵 Azul |
| 3️⃣ **Línea recta** | `x + 8` | x ≥ 3 | 🟢 Verde |

## 🔑 Conceptos clave

### Puntos abiertos y cerrados

En la gráfica verás dos tipos de puntos:

- **⭕ Punto abierto (blanco)**: El punto NO pertenece a ese tramo
  - En x=1: el punto (1, 6) es abierto porque el primer tramo es `x < 1` (sin incluir 1)
  - En x=3: el punto (3, 11) es abierto porque el segundo tramo es `x < 3` (sin incluir 3)

- **⚫ Punto cerrado (negro)**: El punto SÍ pertenece a ese tramo
  - En x=1: el punto (1, 3) es cerrado porque el segundo tramo empieza en `x = 1`
  - En x=3: el punto (3, 11) es cerrado porque el tercer tramo empieza en `x = 3`

## 💡 ¿Cómo funciona el código?

El proceso es bastante simple:

1. **Importar librerías**: NumPy (para números) y Matplotlib (para dibujar)
2. **Crear valores de x**: Separar en tres rangos diferentes
3. **Calcular valores de y**: Aplicar la fórmula correcta a cada rango
4. **Dibujar la gráfica**: Plotear cada tramo con su color
5. **Marcar puntos especiales**: Resaltar dónde se unen los tramos
6. **Embellecer**: Agregar leyenda, título, ejes, cuadrícula, etc.

## 🛠️ Librerías utilizadas

- **NumPy**: Para crear arreglos de números continuos
- **Matplotlib**: Para crear y visualizar gráficas

## 🎨 Lo que verás en la gráfica

- 3 tramos de colores diferentes (rojo, azul y verde)
- Puntos abiertos y cerrados en los puntos de transición
- Líneas punteadas mostrando ejes de simetría
- Cuadrícula para facilitar la lectura
- Leyenda explicando cada elemento

## 📈 Aplicaciones prácticas

Este tipo de funciones las encuentras en:
- **Facturación**: Distintas tarifas según el consumo
- **Impuestos**: Tasas distintas según el ingreso
- **Transporte**: Precios diferentes por tramos de distancia
- **Física**: Modelos con comportamientos diferentes en distintos intervalos

---

**Nota**: Este ejercicio es parte del curso de Cálculo Diferencial de UNAD en Google Colab. 📚✨
