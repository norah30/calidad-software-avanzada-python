# Calidad de Software Avanzada con Python

Portafolio de técnicas avanzadas de calidad y confiabilidad de software, aplicadas a un sistema de admisión hospitalaria. Incluye pruebas combinatorias, mutation testing, análisis estático, cobertura de código y un modelo predictivo de confiabilidad con simulación Monte Carlo.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-testing-green?logo=pytest&logoColor=white)
![sklearn](https://img.shields.io/badge/scikit--learn-ML-red?logo=scikit-learn&logoColor=white)
![Colab](https://img.shields.io/badge/Google-Colab-yellow?logo=googlecolab&logoColor=white)

---

##  Notebooks

### 1.  pruebas_sistema_hospitalario.ipynb

Aplicación de técnicas avanzadas de QA sobre un sistema de admisión hospitalaria.

| Técnica | Herramienta | Resultado |
|---------|-------------|-----------|
| Pruebas combinatorias (pairwise) | `allpairspy` | Reducción de casos con cobertura máxima |
| Priorización por análisis de riesgo | Matriz de riesgo | Casos ordenados por impacto |
| Modelo predictivo de defectos | `sklearn` regresión lineal | Predicción de tasa de fallos |
| Análisis estático de código | `pylint` | Score: 10/10 ✅ |
| Pruebas unitarias + cobertura | `pytest` + `coverage` | **92% de cobertura** |
| Mutation testing | `mutmut` | **78.9% de mutantes eliminados** |
| Pruebas parametrizadas | `pytest.mark.parametrize` | Casos combinatorios automatizados |
| Modelo de confiabilidad | Frestimate | Estimación de confiabilidad por módulo |

---

### 2.  modelo_predictivo_personalisado.ipynb

Modelo personalizado de confiabilidad de software con componente estocástico basado en simulación Monte Carlo.

| Técnica | Detalle |
|---------|---------|
| Dataset sintético | Métricas reales: LOC, complejidad ciclomática, churn de código |
| Feature engineering | Transformaciones logarítmicas (`log1p`) para normalización |
| Modelo base | Regresión lineal sobre log(tasa de defectos) |
| Simulación Monte Carlo | 5000 iteraciones con distribución lognormal + Poisson |
| Output | Score de confiabilidad 0–100 por módulo con intervalos P05–P95 |
| Visualización | Gráficas comparativas de confiabilidad y defectos esperados |

---

##  Tecnologías y librerías

Python 3.x
pytest
coverage
mutmut
allpairspy
pylint
scikit-learn (sklearn)
numpy
scipy
matplotlib
Google Colab


---

##  Ejecutar los notebooks

### En Google Colab (recomendado)

Abre directamente en Colab haciendo clic en el badge:

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/norah30/calidad-software-avanzada-python/blob/main/pruebas_sistema_hospitalario.ipynb)

Ejecuta las celdas en orden con `Shift + Enter`

### En local

```bash
git clone https://github.com/norah30/calidad-software-avanzada-python.git
cd calidad-software-avanzada-python
pip install pytest coverage mutmut allpairspy pylint scikit-learn numpy scipy matplotlib jupyter
jupyter notebook
```

---

##  Resultados destacados

-  **92% de cobertura** de código con `pytest` + `coverage`
-  **78.9% mutation score** con `mutmut`
-  **Score pylint: 10/10** — código limpio y bien estructurado
- Modelo Monte Carlo con **5000 simulaciones** por módulo
-  Reducción de casos de prueba con **pairwise testing** manteniendo cobertura máxima

---


