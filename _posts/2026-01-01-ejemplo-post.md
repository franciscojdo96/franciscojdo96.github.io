---
layout: post
title: "Cómo interpretar la AUC en modelos de riesgo de crédito"
date: 2026-01-01
categories: ["Riesgo Financiero", "Modelos Predictivos"]
tags: ["AUC", "ROCA", "Evaluación"]
description: "Aprende a traducir métricas de clasificación en decisiones de negocio en el ámbito crediticio."
---

Cuando desarrollamos modelos de crédito, tendemos a obsesionarnos con métricas técnicas como la AUC (Área bajo la curva ROC) o la precisión. Pero, ¿qué significan realmente para el negocio y cómo debemos comunicarlas a stakeholders no técnicos?

## De la métrica al impacto

La AUC mide la capacidad del modelo para diferenciar entre deudores buenos y malos【954677612423152†L160-L176】. Una AUC de 0.92 indica que el modelo distingue correctamente en un 92 % de los casos, pero no dice nada sobre costos o beneficios. Para traducir la métrica en impacto debemos considerar:

- **Puntos de corte**: definir umbrales basados en la tolerancia al riesgo y la rentabilidad.
- **Costos de error**: un falso negativo (no identificar un mal pagador) puede ser más costoso que un falso positivo.
- **Contexto regulatorio**: en ciertos mercados, un alto índice de rechazos puede ser observado por entes reguladores.

## Storytelling con datos

Siguiendo la estructura recomendada para presentar modelos de riesgo【954677612423152†L165-L176】:

1. **Contexto**: expón la situación del portafolio de crédito y las implicancias de un modelo deficiente.
2. **Problema**: define claramente qué se quiere optimizar (mora, fraudes, retención) y por qué las aproximaciones actuales no son suficientes.
3. **Tu rol**: destaca tu aporte específico (diseño de variables, selección de modelo, validación, comunicación).
4. **Modelo y métricas**: presenta la AUC junto con métricas de negocio (tasa de aprobación, pérdidas esperadas) y explica cómo se calcularon.
5. **Impacto**: traduce mejoras en métricas en ahorros, ingresos o mejoras en experiencia de cliente.
6. **Visuales**: incluye gráficos simples (curva ROC, ganancias acumuladas) y una frase ejecutiva.

Al contar una historia completa, no solo demostrarás competencia técnica sino también criterio de negocio, lo cual es clave en roles de Data Science y Analytics【994322482176338†L83-L105】.