# Fidelización de Clientes mediante Analítica Predictiva de Abandono en Centros Deportivos

**Proyecto Final Integrador — Minería de Datos (Ciclo Lectivo 2026)**  
*Tecnicatura Superior en Ciencia de Datos e Inteligencia Artificial — IES N° 7 «Populorum Progressio - In.Te.La.»*
*Integrante: Solange Magalí Dominguez*

## Descripción del Proyecto
Sistema analítico de alerta temprana desarrollado bajo la metodología **CRISP-DM** sobre un histórico de 2.000 socios (`clientes_fitness.csv`). El proyecto resuelve cuatro tareas de minería de datos:
1. **Clasificación supervisada:** Detección de socios en riesgo de baja (`Árbol de Decisión max_depth=4`, logrando **87,6% de Recall** y **89,8% de Accuracy** en prueba).
2. **Regresión supervisada:** Proyección de asistencias mensuales esperadas (`Regresión Lineal`, $\text{MAE} = 1,62\text{ clases/mes}$, $R^2 = 0,891$).
3. **Agrupamiento (Clustering):** Segmentación en 3 perfiles operativos mediante `K-Means` y `Clustering Jerárquico Ward` (**97,65%** de concordancia), aislando un clúster crítico que concentra más del 81% de las bajas.
4. **Reglas de asociación:** Extracción de patrones conductuales con `Apriori` (28 reglas, *Lift* máximo de **2,78**).

## Enlaces del Proyecto
* **Tablero Interactivo de Visualización (Lovable):** [Pegar aquí tu enlace .lovable.app]
* **Notebook en Google Colab:** [Pegar aquí el enlace compartido de Colab]

## Estructura del Repositorio
* `MD_Proyecto_Final_Integrador.ipynb`: Notebook reproducible con las 6 etapas CRISP-DM y semilla fija (`random_state=42`).
* `clientes_fitness.csv`: Dataset base original (2.015 registros).
* `tablero_fidelizacion.csv`: Dataset depurado y transformado (2.000 registros).
* `requirements.txt`: Dependencias de Python necesarias para ejecutar el proyecto.

## Instalación y Ejecución Local
```bash
git clone [https://github.com/solddomm/fidelizacion-clientes-mineria-datos.git](https://github.com/solddomm/fidelizacion-clientes-mineria-datos.git)
cd fidelizacion-clientes-mineria-datos
pip install -r requirements.txt
