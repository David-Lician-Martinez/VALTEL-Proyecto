# 📊 Predicción del Precio de Vehículos para la Empresa Telefónica VALTEL

**Autor:** David Licián Martínez  
**Notebook principal:** `VALTEL_Prediccion_Precio_Vehiculos.ipynb`  
**Presentación narrativa:** `VALTEL_Storytelling.pdf`  

---

## 🧠 Introducción

Para el desarrollo de este proyecto se ha optado por seguir la metodología **CRISP-DM (Cross Industry Standard Process for Data Mining)**, un enfoque ampliamente utilizado en ciencia de datos por su carácter estructurado, flexible y adaptable a diferentes dominios.

Esta metodología permite abordar el problema de forma ordenada y comprensible, facilitando la toma de decisiones en cada etapa, desde la comprensión del negocio hasta la evaluación del modelo final. Su carácter cíclico permite revisar decisiones conforme se obtiene nueva información, alineándose perfectamente con el enfoque de **storytelling** que se busca en este trabajo.

---

## 🏢 Contexto empresarial

**Valencian Telecommunications SA (VALTEL)** es una empresa de telecomunicaciones enfocada en ciudadanos no nacionales residentes en España.

En su plan estratégico, VALTEL plantea diversificar servicios e incursionar en el mercado de **coches de segunda mano**, ofreciendo a sus clientes vehículos a precios competitivos desde su app móvil.

Para ello, se plantea como objetivo el desarrollo de un modelo predictivo capaz de **estimar el precio de un vehículo** a partir de sus características técnicas y comerciales.

---

## 🔍 Objetivo del proyecto

El objetivo es construir un modelo de machine learning que permita **predecir el precio** de vehículos de segunda mano. Para ello, se trabajará con un dataset con más de **10.000 registros**, y se aplicará CRISP-DM en todas sus etapas:

- Comprensión del negocio
- Preparación de los datos
- Análisis exploratorio (EDA)
- Modelado con diferentes algoritmos
- Evaluación y selección del modelo más adecuado
- Comunicación de hallazgos mediante storytelling

---

## ⚙️ Metodología y herramientas utilizadas

- Lenguaje: Python
- Visualización: Matplotlib, Seaborn
- Modelos: Decision Tree, Random Forest, XGBoost
- Gestión de nulos: eliminación vs. imputación lógica por subgrupos
- Evaluación: MAE, RMSE, R²
- Presentación: storytelling en PDF

---

## 📈 Resultados del modelado

Se evaluaron varios modelos con dos enfoques de tratamiento de nulos. Se seleccionó el modelo **Árbol de Decisión con imputación de nulos**, por su **alta explicabilidad** y **gran rendimiento**.

| Modelo                          | MAE      | RMSE     | R²     |
|----------------------------------|----------|----------|--------|
| **Random Forest (sin nulos)**   | 4677.43  | 21846.95 | 0.9137 |
| **Random Forest (imputado)**    | 3060.03  |  6332.32 | 0.9826 |
| **Decision Tree (sin nulos)**   | 5124.49  | 23423.72 | 0.9008 |
| **Decision Tree (imputado)**    | 3215.52  |  6707.06 | 0.9805 |
| **XGBoost (sin nulos)**         | 4971.11  | 15680.18 | 0.9556 |
| **XGBoost (imputado)**          | 3404.06  |  6277.15 | 0.9829 |

---

## ✅ Conclusión

El uso de CRISP-DM permitió mantener un flujo de trabajo riguroso, justificado y claro en todas sus fases. Destacamos:

- Una **exploración profunda** de los datos y análisis de outliers
- Dos estrategias de tratamiento de nulos con impacto significativo
- Modelado robusto y validado con métricas de regresión
- Importancia de variables clave como `CV`, `cilindros`, `año`, `consumo` y `mercado`
- Priorización de la **interpretabilidad** en la selección final del modelo

Este proyecto demuestra cómo un enfoque metodológico sólido, combinado con decisiones técnicas bien argumentadas, puede derivar en soluciones aplicables y alineadas con los objetivos de negocio.

---

## 📁 Estructura del repositorio

```
VALTEL-Proyecto/
├── data/              # Datos utilizados
├── notebooks/         # Notebook principal con la metodología completa
├── presentation/      # Storytelling en formato PDF
├── img/               # Gráficos e imágenes usadas en la narrativa
└── README.md          # Este archivo
```

---

## 🧾 Notas finales

Este proyecto fue desarrollado como parte del máster en Ciencia de Datos, con el objetivo de integrar análisis técnico, modelado predictivo y narrativa visual para resolver un caso de negocio realista y aplicable.  
Para cualquier consulta profesional o colaboración, puedes contactarme por LinkedIn:  
**[David Licián Martínez](https://www.linkedin.com/in/david-lician)**


