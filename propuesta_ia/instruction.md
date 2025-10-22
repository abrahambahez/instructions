---
version: 0.1.0
description: Esquema de propuesta a cliente a partir de datos de negocio y agente virtual
lang: es
tags:
  - silia
  - labor
---

You will be provided with a business analysis document and agent ideas to create an executive business case in Spanish for virtual AI agents.

Here is the business analysis document:
<business_analysis>
{{analysis}}
</business_analysis>

Here are the agent ideas:
<agent_ideas>
{{input|ideas}}
</agent_ideas>

Your task is to write an **executive business case in Markdown format** using the information provided in the business analysis and agent ideas.

## Requirements:

- Use a **casual business tone** - serious but direct and persuasive
- Use clear language, short sentences focused on business value
- The document must be **very brief, concise and executive** as it will be used in a presentation (each section will be a slide)
- **Do not invent information under any circumstances**
- If any data is not present in the analysis, use the following placeholder format: `[especificar: detalle a especificar]`

## Instructions:

1. Read both the business analysis document and agent ideas provided as input
2. Identify only essential information: problem, process, metrics, impact, benefits
3. Write the business case **following the exact structure shown below**
4. If the input does not contain information for a section, place a placeholder using the indicated format
5. Return the text in Markdown format, without additional explanations or comments

## Exact Structure to Follow:

### 1. Contexto del cliente
Describe brevemente la situación actual del cliente.
- Qué proceso o área presenta fricción o ineficiencia.
- Por qué es relevante resolverlo ahora.
- Qué objetivos estratégicos se beneficiarían.

### 2. El desafío actual
Resume el problema de forma concreta y cuantificable.
- Recursos invertidos actualmente (personas, tiempo, costo, errores)
- Impacto operativo o financiero
- Consecuencias en la experiencia o cumplimiento

### 3. La oportunidad
Explica el cambio posible al adoptar la solución.
- Qué ganaría el cliente al automatizar o transformar el proceso.
- Cómo mejora indicadores clave (flujo, tiempos, productividad, satisfacción).
- Incluye una frase de valor: "Convertir el cuello de botella operativo en una ventaja competitiva".

### 4. La solución propuesta
Describe el agente virtual o sistema de IA de forma clara y no técnica.
- Qué hace y cómo se integra al flujo actual.
- Qué lo diferencia de una automatización convencional.
- Qué resultados genera de forma medible o inmediata.

### 5. Componentes principales
Enumera los módulos o capacidades clave del agente virtual.
Cada componente con descripción y beneficio directo.

#### 1. [especificar: nombre del componente]
Descripción breve.
**Beneficio:** [especificar: beneficio directo]

#### 2. [especificar: nombre del componente]
Descripción breve.
**Beneficio:** [especificar: beneficio directo]

#### 3. [especificar: nombre del componente]
Descripción breve.
**Beneficio:** [especificar: beneficio directo]

### 6. Impacto esperado
Resultados expresados en términos de negocio.

| Indicador | Situación actual | Con agente virtual | Mejora estimada |
|------------|------------------|--------------------|-----------------|
| Tiempo de procesamiento | [especificar] | [especificar] | [especificar] |
| FTE dedicados | [especificar] | [especificar] | [especificar] |
| Flujo de caja (DSO) | [especificar] | [especificar] | [especificar] |
| Costos operativos | [especificar] | [especificar] | [especificar] |

### 7. Plan de implementación
Describe las fases esenciales y el esfuerzo estimado.

**Fases:**
1. Diagnóstico y levantamiento del flujo actual
2. Diseño y configuración inicial del agente virtual
3. Integraciones y pruebas piloto
4. Despliegue y seguimiento de métricas

**Duración estimada:** [especificar]
**Recursos requeridos del cliente:** [especificar]
**Soporte:** [especificar]

### 8. Costos y retorno estimado
Resume la inversión y beneficios esperados.

| Concepto | Monto estimado | Frecuencia |
|-----------|----------------|-------------|
| Implementación inicial | [especificar] | Único |
| Licencia o mantenimiento | [especificar] | Mensual |
| Soporte o mejora continua | [especificar] | Mensual |

**Ahorro proyectado:** [especificar]
**Periodo de recuperación estimado:** [especificar]

### 9. Equipo del proyecto
Identifica a los responsables principales.

| Nombre | Rol | Responsabilidad |
|---------|-----|-----------------|
| [especificar] | [especificar] | [especificar] |
| [especificar] | [especificar] | [especificar] |
| [especificar] | [especificar] | [especificar] |

### 10. Próximos pasos
Define las siguientes acciones y tiempos sugeridos.

**Siguientes hitos:**
- [especificar: acción siguiente]
- [especificar: acción siguiente]
- [especificar: acción siguiente]

**Plazo estimado:** [especificar]
**Responsables:** [especificar]

Return only the completed business case in Markdown format following this exact structure. Use the placeholder format `[especificar: detalle a especificar]` for any missing information.
