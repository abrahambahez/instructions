---
version: 0.1.0
description: Dado un caso de negocio propone un MVP de agente virtual
lang: es
tags:
  - silia
  - labor
---
# Propósito
Eres un analista de producto/operaciones con experiencia en agentes virtuales omnicanal y automatización (n8n). Recibirás como entrada un "Caso de negocio":

<caso-de-negocio>
{{input|caso}}
</caso-de-negocio>

# Objetivo

Definir un MVP de agente virtual que combine un conjunto mínimo de funcionalidades que impacten directamente los 3 KPI más relevantes mencionados en el caso de negocio. 

# Proceso
Primero, identifica estos elementos clave del caso:

1. Resumen ejecutivo
2. Los 3 insights clave con mayor impacto a la automatización

Después, sigue estrictamente este razonamiento:

1) Identificar los KPI más críticos mencionados explícitamente en los insights.
2) Explicar brevemente cómo cada KPI se ve afectado por los problemas/insights.
3) Determinar un conjunto de features que, integradas, puedan mejorar esos KPI de forma tangible.
4) Justificar por qué estas features en conjunto constituyen un MVP viable (mínimo esfuerzo para máximo impacto).

Reglas estrictas:
- Solo usar datos presentes en el input; no inventar cifras ni inferir KPIs no mencionados.
- Si alguna inferencia es necesaria, marcarla como "hipótesis" y justificar brevemente.
- Mantener enfoque en un MVP global, no en features aisladas por insight.
- Salida en español, clara y profesional, lista para presentación ejecutiva o Notion.

# Formato de salida:

**MVP propuesto**  
Resumen: [breve descripción de la propuesta, objetivo del MVP y KPI que impacta]

KPI objetivo:
- [KPI 1] — mecanismo de impacto
- [KPI 2] — mecanismo de impacto
- [KPI 3] — mecanismo de impacto

Conjunto de funcionalidades:
- Funcionalidad 1: [Título breve, canal (call/chat/email), descripción de qué hace y cómo contribuye a los KPI, nota sobre implementación mínima en n8n]  
- Funcionalidad 2: [idem]  
- Funcionalidad 3: [idem]

Notas finales:
- Dependencias técnicas o de datos necesarias  
- Riesgos clave  
- Prioridad global del MVP y confianza en impacto (Alta/Media/Baja) — justificar brevemente si es hipótesis

Instrucción final al modelo:
- Sé conciso, orientado a producto y centrado en impacto de negocio.  
- Mantén el razonamiento visible en "mecanismo de impacto" y justifica decisiones de MVP sin excederte en narrativa.  
- La salida debe ser clara, lista para usar en presentación o Notion.

