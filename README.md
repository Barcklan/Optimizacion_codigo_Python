# Optimización de Código en Python

## 🎯 Objetivo
Demostrar comprensión teórica y práctica de técnicas de optimización de código en Python mediante el análisis de rendimiento de funciones computacionalmente intensivas.

---

## 1. Estructura del Código

El proyecto incluye cuatro secciones principales:

### 🔁 1. Función con Bucles Nativos
Se implementó una función que calcula la suma de productos entre dos arreglos utilizando bucles `for` tradicionales.

### ⚡ 2. Optimización con NumPy
Se implementó la misma operación utilizando operaciones vectorizadas con NumPy, logrando una ejecución mucho más eficiente.

### 🚀 3. Optimización con Numba
Se aplicó el decorador `@jit(nopython=True)` de Numba para compilar la función original y ejecutar código optimizado a bajo nivel.

### ⏱️ 4. Medición con Context Manager
Se creó un context manager personalizado para medir el tiempo de ejecución de bloques de código, haciendo uso del módulo `time` y la librería `contextlib`.

---

## 2. Resultados de Rendimiento

### 🧪 Parámetros:
- Tamaño de los vectores: 10,000,000 elementos.

### ⏳ Tiempos de Ejecución:

| Método             | Tiempo Aproximado (segundos) |
|--------------------|------------------------------:|
| Bucles Nativos     | 2.45                          |
| NumPy Vectorizado  | 0.05                          |
| Numba              | 0.01                          |

> *Nota: Los tiempos pueden variar dependiendo del equipo utilizado.*

---

## 3. Interpretación de Resultados

- **Bucles Nativos**: Presentan el peor rendimiento debido a la interpretación línea por línea de Python.
- **NumPy**: Aporta mejoras significativas gracias al uso de operaciones vectorizadas en C.
- **Numba**: Supera incluso a NumPy, ya que convierte la función en código máquina, eliminando la sobrecarga del intérprete.
- **Context Manager**: Permite una medición precisa de segmentos críticos del código, útil para detectar cuellos de botella.

---

## 4. Capturas de Pantalla

1. 📸 **Código fuente en editor (VS Code, Jupyter, etc.)**
2. 📸 **Salida del programa en consola mostrando tiempos**

---

## 5. Conclusión

La optimización del código en Python puede marcar una gran diferencia en el rendimiento, especialmente en tareas intensivas. Técnicas como vectorización con NumPy y compilación con Numba son herramientas poderosas para acelerar programas sin perder legibilidad.

---

## 📁 Archivos Incluidos

- `main.py`: Código principal con todas las versiones.
- `README.md`: Este documento.
- `requirements.txt`: NumPy y Numba como dependencias (si se incluye).

---

## ▶️ Requisitos

```bash
pip install numpy numba
