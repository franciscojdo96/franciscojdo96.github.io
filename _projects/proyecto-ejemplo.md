---
title: "Modelo de Detección de Fraude en Tarjetas"
date: 2025-11-30
industry: "Fintech"
role: "Data Scientist Líder"
metrics: "23% de incremento en la tasa de detección, reducción de falsas alarmas en 15%"
summary: "Diseñé e implementé un modelo de scoring de riesgo de fraude que aumentó la detección de transacciones fraudulentas y redujo las falsas alarmas, ahorrando millones de dólares en pérdidas."
context: |
  **Contexto del Negocio**
  
  La empresa procesaba 2 millones de transacciones diarias y sufría de un alto porcentaje de falsos positivos en su motor basado en reglas, lo que impactaba la experiencia del cliente y generaba pérdidas por transacciones no completadas.
problem: |
  **Problema**
  
  El sistema de reglas existente marcaba el 30 % de las transacciones legítimas como sospechosas, ocasionando $2 M en pérdidas trimestrales y generando desgaste en la atención al cliente. Se necesitaba un modelo que balanceara detección y minimizara falsas alarmas.
solution: |
  **Solución Técnica**
  
  Lideré el diseño de un modelo de árboles de gradiente (XGBoost) con ingeniería de 12 nuevas variables comportamentales. Utilicé validación cruzada 5‑fold para evaluar múltiples modelos y seleccioné XGBoost por su AUC de 0.92 (vs. 0.85 del baseline). Implementé un panel de interpretabilidad con SHAP para explicar las predicciones a equipos no técnicos.
impact: |
  **Impacto Cuantificado**
  
  * 23 % de incremento en la tasa de detección de fraude
  * 15 % de reducción en falsas alarmas, ahorro anual de $1.2 M
  * Aumento del 4 % en retención de clientes gracias a menor fricción

links:
  - name: "Repositorio del proyecto"
    url: "https://github.com/usuario/proyecto-fraude"
  - name: "Presentación ejecutiva"
    url: "https://example.com/presentacion-fraude.pdf"
---

<!--
Esta plantilla muestra cómo estructurar un proyecto en el sitio. Cada sección usa variables en el front matter para que el layout pueda presentar la información de forma coherente. Para crear un nuevo proyecto, copia este archivo dentro de la carpeta `_projects` y reemplaza los campos con tu contenido.
-->

El cuerpo del archivo puede usarse para proporcionar detalles adicionales, como notas técnicas, hallazgos o aprendizajes. Este texto aparecerá al final de la página de proyecto después de las secciones predefinidas.