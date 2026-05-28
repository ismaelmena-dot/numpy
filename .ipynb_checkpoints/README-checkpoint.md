# 🧪 NumPy & Procesamiento de Imágenes en Python

Un espacio dedicado al aprendizaje práctico de **NumPy**, manipulación de arreglos multidimensionales y análisis básico de imágenes utilizando Python y Jupyter Notebooks.

Este repositorio contiene scripts y libretas interactivas diseñadas para explorar los conceptos fundamentales de la computación científica y el procesamiento de imágenes digitales.

---

## 📁 Estructura del Proyecto

El repositorio está organizado de la siguiente manera:

```text
numpy/
├── prueba.ipynb         # Generación y formateo de matrices aleatorias con Python puro
├── prueba2.ipynb        # Análisis y lectura de imágenes (beagle.jpg) con Matplotlib
├── x.ipynb              # Introducción práctica a arreglos de NumPy (dimensiones, shapes y tipos)
├── beagle.jpg           # Imagen de muestra utilizada para el análisis visual
└── .venv/               # Entorno virtual con las dependencias del proyecto instaladas
```

---

## 📓 Descripción de los Notebooks

### 1. 🧮 `x.ipynb` - Introducción a NumPy
Este notebook sirve como punto de partida para entender cómo funciona la estructura central de NumPy: el `ndarray` (arreglo multidimensional).
* **Conceptos clave:**
  * Creación de arreglos a partir de listas anidadas con `np.array()`.
  * Definición explícita de tipos de datos en la creación de arreglos (`dtype='float'`).
  * Inspección de atributos fundamentales de arreglos para comprender su anatomía:
    * `.ndim`: Cantidad de dimensiones o ejes.
    * `.shape`: Dimensiones del arreglo en formato de tupla `(filas, columnas)`.
    * `.size`: Cantidad total de elementos dentro de la estructura.

### 2. 🔢 `prueba.ipynb` - Generación de Matrices Aleatorias
En este cuaderno se explora la creación y visualización de matrices cuadradas utilizando estructuras de Python estándar y generación aleatoria básica.
* **Conceptos clave:**
  * Generación dinámica de matrices cuadradas de tamaño $N \times N$ usando números aleatorios enteros (`random.randint`).
  * Formateo avanzado de impresión en consola para que las matrices mantengan una alineación visual perfectamente simétrica (empleando f-strings `:2` y `.join()`).
  * Pruebas interactivas con matrices generadas de dimensiones: $5 \times 5$, $10 \times 10$ y $20 \times 20$.

### 3. 🖼️ `prueba2.ipynb` - Análisis de una Imagen con Matplotlib
Aquí se da el salto al procesamiento digital de imágenes, demostrando de manera práctica cómo una imagen rasterizada se representa nativamente como una matriz de tres dimensiones en memoria.
* **Conceptos clave:**
  * Lectura de imágenes en disco (`beagle.jpg`) mediante la función `plt.imread()` de la librería Matplotlib.
  * Análisis de la resolución y canales de color usando `.shape` para revelar la estructura `(Alto, Ancho, Canales de color RGB)`.
  * Acceso directo a coordenadas específicas e inspección de valores numéricos de píxeles individuales (representados en canales Rojo, Verde y Azul con valores en rango $[0, 255]$).

---

## 🛠️ Requisitos e Instalación

Para ejecutar estos notebooks de forma local, puedes aprovechar el entorno virtual provisto o configurar uno nuevo paso a paso.

### Dependencias Principales
El proyecto requiere las siguientes librerías de Python:
* **NumPy** (`numpy`): Para cálculo numérico de alto rendimiento y manipulación de arreglos eficientes.
* **Matplotlib** (`matplotlib`): Para lectura, procesamiento y visualización de imágenes, y generación de gráficos.
* **Jupyter** (`notebook` / `jupyterlab`): Para ejecutar y experimentar en las libretas interactivas `.ipynb`.

### Configuración del Entorno

1. **Clonar o acceder al directorio del proyecto:**
   ```bash
   cd numpy
   ```

2. **Activar el entorno virtual existente (`.venv`):**
   * **macOS/Linux:**
     ```bash
     source .venv/bin/activate
     ```
   * **Windows:**
     ```cmd
     .venv\Scripts\activate
     ```

3. **Instalar dependencias** (en caso de usar un entorno nuevo o limpio):
   ```bash
   pip install numpy matplotlib notebook
   ```

4. **Iniciar el servidor de Jupyter:**
   ```bash
   jupyter notebook
   ```

---

## 🚀 ¿Cómo empezar?

1. Abre `x.ipynb` para familiarizarte con las propiedades básicas de los arreglos multidimensionales en NumPy.
2. Continúa con `prueba.ipynb` para observar la generación lógica de matrices y la estructura visual de formateo personalizado.
3. Finalmente, abre `prueba2.ipynb` para cargar `beagle.jpg` y ver cómo se representa visualmente una matriz de tres dimensiones que contiene información de color RGB real de una fotografía.

---
> [!NOTE]
> Este proyecto forma parte de una ruta de aprendizaje orientada a **Ciencia de Datos**, **Computación Científica** y **Procesamiento de Imágenes**. ¡Perfecto para entusiastas del análisis de datos que inician su viaje en Python!
