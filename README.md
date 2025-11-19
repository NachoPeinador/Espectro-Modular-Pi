# El Espectro Modular de $\pi$: De la Estructura de Canales Primos a las Supercongruencias Elípticas

[![License](https://img.shields.io/badge/License-AGPLv3_+_Enterprise-blueviolet.svg)](LICENSE-AGPL.md)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626.svg?style=flat&logo=Jupyter)](TEOREMA_DE_REPRESENTACIÓN_MODULAR_DE_π.ipynb)

**Autor:** José Ignacio Peinador Sala  
**Contacto:** [joseignacio.peinador@gmail.com](mailto:joseignacio.peinador@gmail.com)  
**ORCID:** [0009-0008-1822-3452](https://orcid.org/0009-0008-1822-3452)

---

## 📜 Resumen del Proyecto

Este repositorio contiene el código fuente, los datos experimentales y el manuscrito del artículo de investigación **"El Espectro Modular de $\pi$"**.

Este trabajo propone una unificación inédita entre el análisis clásico y la teoría de números, demostrando que la constante $\pi$ no es una estructura monolítica, sino que posee una **"Uniformidad Modular"** que se manifiesta en tres escalas:
1.  **Baja Energía:** Una representación lineal basada en los canales primos $6k \pm 1$.
2.  **Alta Energía:** Series de convergencia exponencial (tipo Ramanujan-Sato, Nivel 58) derivadas mediante el algoritmo PSLQ.
3.  **Aritmética Local:** Propiedades de "holografía aritmética" verificadas mediante algoritmos Spigot y supercongruencias en cuerpos finitos.

---

## 📂 Estructura del Repositorio

* **`Paper/`**: Contiene el manuscrito científico en formato PDF y los archivos fuente LaTeX.
    * `main_v2.tex`: Archivo principal del artículo.
* **`Notebooks/`**: Notebooks de Jupyter/Colab con la validación computacional.
    * `TEOREMA_DE_REPRESENTACIÓN_MODULAR_DE_π.ipynb`: El "núcleo" experimental. Incluye la derivación de la serie modular, las pruebas de convergencia y la validación de la fórmula de Euler.
* **`Code/`**: Implementaciones puras en Python de los algoritmos clave.
    * `modular_pi.py`: Calculadora de la serie $6k \pm 1$.
    * `spigot_bbp.py`: Implementación del algoritmo de extracción hexadecimal.

---

## 🚀 Principales Hallazgos

### 1. La Serie Modular de $\pi$
Demostramos algebraicamente y verificamos computacionalmente que $\pi$ emerge de la interferencia constructiva en los canales modulares $1$ y $5 \pmod 6$:

$$\pi = 3 \sum_{k=0}^{\infty} (-1)^k \left( \frac{1}{6k+1} + \frac{1}{6k+5} \right)$$

### 2. Convergencia Exponencial (Nivel 58)
Mediante matemáticas experimentales (algoritmo PSLQ con 200 dígitos de precisión), reconstruimos la serie de Ramanujan asociada al discriminante $d = -232$, validando una tasa de convergencia de $\approx 8$ dígitos por término.

### 3. Dualidad Computacional
Implementamos algoritmos Spigot que demuestran la propiedad de "localidad" de $\pi$, permitiendo extraer el $n$-ésimo dígito hexadecimal sin calcular los anteriores, una manifestación de la estructura modular subyacente.

---

## 💻 Reproducibilidad

Todos los resultados presentados en el artículo son reproducibles.

### Requisitos
* Python 3.8+
* Librerías: `numpy`, `scipy`, `mpmath`, `matplotlib`

### Ejecución Rápida
Para replicar los experimentos de convergencia y validación de fórmulas, ejecute el notebook principal:

```bash
jupyter notebook Notebooks/ESPECTRO_MODULAR_π.ipynb
