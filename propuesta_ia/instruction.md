---
version: 0.1.0
description: Esquema de propuesta a cliente a partir de datos de negocio y agente virtual
lang: es
tags:
  - silia
  - labor
---

Se te proporcionará un documento de análisis de negocio e ideas de agentes para crear un caso de negocio ejecutivo en español para agentes virtuales de IA.

Aquí está el documento de análisis de negocio:

<business_analysis>
{{analysis}}
</business_analysis>

Aquí están las ideas de agentes:

<agent_ideas>
{{input|ideas}}
</agent_ideas>

Tu tarea es escribir un **caso de negocio ejecutivo en formato Markdown** utilizando la información proporcionada en el análisis de negocio y las ideas de agentes.

## Requirements:

- Utiliza un **tono de negocio informal** - serio pero directo y persuasivo
- Utiliza un lenguaje claro, frases cortas centradas en el valor de negocio
- El documento debe ser **muy breve, conciso y ejecutivo** ya que se utilizará en una presentación (cada sección será una diapositiva)
- **No inventes información bajo ninguna circunstancia**
- Si algún dato no está presente en el análisis, utiliza el siguiente formato de marcador de posición: `[especificar: detalle a especificar]`

## Instructions:

1. Lee tanto el documento de análisis de negocio como las ideas de agentes proporcionadas como entrada
2. Identifica solo la información esencial: problema, proceso, métricas, impacto, beneficios
3. Escribe el caso de negocio **siguiendo la estructura exacta mostrada a continuación**
4. Si la entrada no contiene información para una sección, coloca un marcador de posición utilizando el formato indicado
5. Devuelve el texto en formato Markdown, sin explicaciones ni comentarios adicionales

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

Devuelve solo el caso de negocio completado en formato Markdown siguiendo esta estructura exacta. Utiliza el formato de marcador de posición `[especificar: detalle a especificar]` para cualquier información faltante.
