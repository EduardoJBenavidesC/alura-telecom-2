# alura-telecom-2
Proyecto para especialización en Data Science  ML
Entendido. Ajuste de última hora realizado para que el `README.md` refleje exactamente el nombre del archivo final y mantenga el rigor técnico del desafío.

Aquí tienes la versión definitiva, sobria y orientada a la ingeniería del proyecto:

---

# Technical Pipeline: Predictive Churn Architecture

**Lead Data Scientist:** Eduardo J. Benavides C.

**Stack:** Python | Scikit-Learn | Imbalanced-Learn | MDM Layer

**Project:** Allura Telecom Challenge (Final Audit)

---

### I. REQUERIMIENTOS TÉCNICOS Y DESAFÍO

El proyecto aborda la detección temprana de fuga de clientes bajo un escenario de clases desbalanceadas. El desafío principal consistió en la construcción de un pipeline robusto capaz de mitigar el ruido en la ingesta y garantizar la generalización del modelo en entornos de producción.

### II. HITOS DE INGENIERÍA Y CONTROL

El flujo se estructura en cuatro capas de procesamiento auditadas:

1. **MDM & Data Cleansing:** * Tratamiento de inconsistencias en registros de facturación.
* Inyección de lógica de negocio para filtrado de leads obsoletos.


2. **Feature Engineering:**
* Implementación de *One-Hot Encoding* para variables categóricas de alta cardinalidad (Servicios e Internet).
* Estandarización de variables numéricas mediante `StandardScaler`.


3. **H-AUDIT (Control de Sesgo):**
* Aplicación de **SMOTE** para el balanceo sintético de la variable objetivo.
* Validación de la capacidad de aprendizaje mediante **Learning Curves**, confirmando la convergencia en el umbral de **0.80**.


4. **Tuning & Modelado:**
* Optimización de hiperparámetros mediante `RandomizedSearchCV` para la selección del *Champion Model*.



### III. INFRAESTRUCTURA DEL MODELO

* **Algoritmo:** Random Forest Classifier (Optimizado).
* **Métrica de Optimización:** Recall (Sensibilidad) para la captura máxima de desertores.
* **Evaluación Final:** ROC-AUC de **0.8214** y Recall de **67.65%**.

### IV. ESTRUCTURA DEL REPOSITORIO

* `Allura_Telecom_Proy_VF.ipynb`: Pipeline técnico completo y auditado.
* `modelo_champion_telecom_vf.pkl`: Activo atómico (binario) final para integración B2B.
* `Presentacion_Ejecutiva_Churn_Benavides.pdf`: Informe de impacto y estrategias de negocio.

---

**Certificación de Auditoría:** Este repositorio cumple con los estándares de trazabilidad y rigor técnico exigidos. Las cifras reportadas coinciden estrictamente con los logs de ejecución del sistema.

---

**Corre, quedan los últimos minutos. ¡Éxito con la subida!**
