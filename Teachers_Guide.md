# 🍎 Teacher's Guide: The Modular Spectrum of $\pi$

## Pentalogy of Interactive STEM Workshops

### 1. Introduction
This guide accompanies the 5 interactive notebooks of the project. The pedagogical objective is to foster computational thinking and mathematical intuition, moving away from rote memorization.

> **Reference:** Peinador Sala, J. I. (2025). *The Modular Spectrum of π*. Zenodo.

📄 **[Download Teacher's Guide in PDF (for printing)](https://github.com/NachoPeinador/Espectro-Modular-Pi/blob/main/Docs/Teachers_guide.pdf)**

---

### 2. Session Breakdown

#### 📘 Session 1: Arithmetic and Patterns [Open Notebook](https://colab.research.google.com/github/NachoPeinador/Espectro-Modular-Pi/blob/main/Notebooks/🕵️‍♂️ Unlocking the Secrets of π.ipynb)
* **Focus:** Understanding that not all algorithms are created equal.
* **Key Point:** The **"Modular Clock"**. Students must visualize that prime numbers (and useful terms of $\pi$) only exist in channels $1$ and $5$ of modulo $6$.
* **❓ FAQ:** *"Why is 25 on the list if it's not prime?"*
    * **Answer:** In the modular sum, we filter numbers coprime to 6 (not even, not multiples of 3). 25 fulfills this condition. In the Euler product (Session 2), we will be stricter.

#### 🔗 Session 2: Deep Connections [Open Notebook](https://colab.research.google.com/github/NachoPeinador/Espectro-Modular-Pi/blob/main/Notebooks/El_Universo_Conectado_de_π_Probabilidad,_Complejos_y_Misterios.ipynb)
* **Focus:** The omnipresence of $\pi$.
* **⭐ Star Activity:** Calculate the area of the Bell Curve (Gaussian) using a series of simple fractions. This is a very powerful moment of interdisciplinary connection.
* **💬 Debate:** Compare the modular formula (slow but understandable) with Ramanujan's (fast but obscure). Discuss *"Efficiency vs. Explainability"*.

#### 🌍 Session 3: Application and Geometry [Open Notebook](https://colab.research.google.com/github/NachoPeinador/Espectro-Modular-Pi/blob/main/Notebooks/π_en_Acción_Geometría,_Dimensiones_y_lo_Imposible.ipynb)
* **Focus:** Error propagation.
* **Analogy:** **"Losing the Mediterranean Sea"**. When calculating the volume of the Earth ($r^3$), a decimal error in $\pi$ is magnified cubically.
* **Monte Carlo:** Visual demonstration that chance (brute force) is computationally inefficient compared to an ordered mathematical structure.

#### ⚙️ Session 4: Engineering and Algorithms [Open Notebook](https://colab.research.google.com/github/NachoPeinador/Espectro-Modular-Pi/blob/main/Notebooks/Las_Herramientas_del_Infinito.ipynb)
* **Focus:** Practical utility.
* **🔐 Cryptography:** The "Prime Benchmark" demonstrates that skipping useless modular channels (0, 2, 3, 4) accelerates prime number search by **~33%**. This is vital in cybersecurity.
* **Basel Problem:** Numerical resolution of $\sum 1/n^2 = \pi^2/6$ using the square of the modular series.

#### 🧬 Session 5: Abstract Theory [Open Notebook](https://colab.research.google.com/github/NachoPeinador/Espectro-Modular-Pi/blob/main/Notebooks/El_Código_Fuente_de_las_Matemáticas.ipynb)
* **Focus:** Paradigm Shift.
* **🌻 Fibonacci:** Discovery of the 24-step cycle (**Pisano Period**) in nature.
* **Modular Matrix:** Visualization of "strong interactions" (prime channel crossings) in matrices, suggesting hidden structures in linear algebra.

---

### 3. Challenge Solutions

| Challenge | Colab | Approximate Solution |
| :--- | :---: | :--- |
| **6 Decimals of $\pi$** | 1 | **~500,000 terms** are needed due to linear convergence $O(1/N)$. |
| **Monte Carlo vs Modular** | 3 | To match the precision of the modular method with 100 terms, Monte Carlo would require **millions of points** (convergence $1/\sqrt{N}$). |
| **Factorial of 0.5** | 3 | The result is $\sqrt{\pi}/2 \approx 0.8862$. |

---

### 4. Technical Requirements
No local software installation is required. The workshops are designed to run in the cloud.

* **Platform:** Google Colab.
* **Python Libraries:** `numpy`, `matplotlib`, `mpmath`.
