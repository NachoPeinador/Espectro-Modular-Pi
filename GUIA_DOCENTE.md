# 🍎 Guía del Profesor: El Espectro Modular de $\pi$

## Pentalogía de Talleres Interactivos para STEM

### 1. Introducción
Esta guía acompaña a los 5 cuadernos interactivos del proyecto. El objetivo pedagógico es fomentar el pensamiento computacional y la intuición matemática, alejándose de la memorización mecánica.

> **Referencia:** Peinador Sala, J. I. (2025). *The Modular Spectrum of π*. Zenodo.

---

### 2. Desglose por Sesiones

#### 📘 Sesión 1: Aritmética y Patrones [Abrir cuaderno](https://colab.research.google.com/github/NachoPeinador/Espectro-Modular-Pi/blob/main/Notebooks/Desbloqueando_los_Secretos_de_π.ipynb)
* **Foco:** Entender que no todos los algoritmos son iguales.
* **Punto Clave:** El **"Reloj Modular"**. Los alumnos deben visualizar que los números primos (y los términos útiles de $\pi$) solo existen en los canales $1$ y $5$ del módulo $6$.
* **❓ Duda Frecuente:** *"¿Por qué el 25 está en la lista si no es primo?"*
    * **Respuesta:** En la suma modular, filtramos números coprimos con 6 (no pares, no múltiplos de 3). El 25 cumple esto. En el producto de Euler (Sesión 2) seremos más estrictos.

#### 🔗 Sesión 2: Conexiones Profundas [Abrir cuaderno](Notebooks/El_Universo_Conectado_de_π_Probabilidad,_Complejos_y_Misterios.ipynb)
* **Foco:** La omnipresencia de $\pi$.
* **⭐ Actividad Estrella:** Calcular el área de la Campana de Gauss (Estadística) usando una serie de fracciones simples. Es un momento de conexión interdisciplinar muy potente.
* **💬 Debate:** Comparar la fórmula modular (lenta pero comprensible) con la de Ramanujan (rápida pero oscura). Discutir *"Eficiencia vs. Explicabilidad"*.

#### 🌍 Sesión 3: Aplicación y Geometría [Abrir cuaderno](Notebooks/π_en_Acción_Geometría,_Dimensiones_y_lo_Imposible.ipynb)
* **Foco:** La propagación del error.
* **Analogía:** **"Perder el Mar Mediterráneo"**. Al calcular el volumen de la Tierra ($r^3$), un error decimal en $\pi$ se magnifica cúbicamente.
* **Monte Carlo:** Demostración visual de que el azar (fuerza bruta) es computacionalmente ineficiente comparado con una estructura matemática ordenada.

#### ⚙️ Sesión 4: Ingeniería y Algoritmos [Abrir cuaderno](Notebooks/Las_Herramientas_del_Infinito.ipynb)
* **Foco:** Utilidad práctica.
* **🔐 Criptografía:** El "Benchmark de Primos" demuestra que saltarse los canales modulares inútiles (0, 2, 3, 4) acelera la búsqueda de números primos en un **~33%**. Esto es vital en seguridad informática.
* **Problema de Basilea:** Resolución numérica de $\sum 1/n^2 = \pi^2/6$ usando el cuadrado de la serie modular.

#### 🧬 Sesión 5: Teoría Abstracta [Abrir cuaderno](Notebooks/El_Código_Fuente_de_las_Matemáticas.ipynb)
* **Foco:** Cambio de Paradigma.
* **🌻 Fibonacci:** Descubrimiento del ciclo de 24 pasos (**Periodo de Pisano**) en la naturaleza.
* **Matriz Modular:** Visualización de las "interacciones fuertes" (cruces de canales primos) en matrices, sugiriendo estructuras ocultas en el álgebra lineal.

---

### 3. Solucionario de Retos

| Reto | Colab | Solución Aproximada |
| :--- | :---: | :--- |
| **6 Decimales de $\pi$** | 1 | Se necesitan **~500,000 términos** debido a la convergencia lineal $O(1/N)$. |
| **Monte Carlo vs Modular** | 3 | Para igualar la precisión del método modular con 100 términos, Monte Carlo requeriría **millones de puntos** (convergencia $1/\sqrt{N}$). |
| **Factorial de 0.5** | 3 | El resultado es $\sqrt{\pi}/2 \approx 0.8862$. |

---

### 4. Requisitos Técnicos
No se requiere instalación de software local. Los talleres están diseñados para ejecutarse en la nube.

* **Plataforma:** Google Colab.
* **Librerías Python:** `numpy`, `matplotlib`, `mpmath`.
