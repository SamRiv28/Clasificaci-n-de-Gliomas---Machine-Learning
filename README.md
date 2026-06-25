# Clasificación de Gliomas Cerebrales mediante Aprendizaje Automático

**Materia:** Aprendizaje Automático  
**Autora:** Sandra Rivera  
**Universidad:** Universidad Autónoma del Estado de Morelos  

---

## Descripción

Este proyecto aplica técnicas de aprendizaje automático supervisado para predecir 
el grado de gliomas cerebrales — tumores primarios del sistema nervioso central — 
clasificándolos en bajo grado (LGG) o alto grado (HGG) a partir de características 
clínicas y genómicas de pacientes reales.

---

## Dataset

**Nombre:** Glioma Grading Clinical and Mutation Features  
**Fuente:** UCI Machine Learning Repository  
**ID:** 759  
**Referencia:** Tasci, E., Camphausen, K., Krauze, A., & Zhuge, Y. (2022). https://doi.org/10.24432/C5R62J  

| Característica | Valor |
|---|---|
| Instancias | 839 pacientes |
| Variables | 23 (3 clínicas + 20 mutaciones genéticas) |
| Variable objetivo | Grade: LGG (0) / HGG (1) |
| Valores faltantes | Ninguno |

> El dataset se descarga automáticamente al correr el notebook 
> usando la librería `ucimlrepo`. No es necesario descargarlo manualmente.

---

## Modelos Comparados

| Modelo | Accuracy | Recall HGG | AUC |
|---|---|---|---|
| Regresión Logística | 86.31% | 89% | 0.9207 |
| SVM | 87.50% | 94% | 0.8787 |
| Random Forest | 78.57% | 74% | 0.9010 |

**Modelo ganador:** SVM — mejor accuracy y mejor recall de HGG, 
que es la métrica más importante clínicamente.

---

## Estructura del Repositorio
