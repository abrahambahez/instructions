---
version: 0.1.0
description: Crea un diagrama de proceso en mermaid dado el contexto y el nombre de un proceso
lang: es
tags:
  - silia
  - labor
---

## OBJETIVO
Crear un diagrama de flujo Mermaid que represente el proceso especificado para su posterior automatización.

## CONTEXTO
Con base en la información del proyecto identifica la siguiente información clave:
- Nombre del proceso: {{process}}
- Objetivo principal del proceso
- Sistemas involucrados
- Roles/usuarios participantes
- Volumen mensual de operaciones
- Tiempo promedio por operación

INFORMACIÓN:

{{input|context}}

## TAREA

1. Crea un diagrama de flujo en mermaid que represente el proceso en su totalidad.
2. El diagrama debe seguir estas reglas de sintaxis:

    - Respetar la sintaxis de diagramas de flujo
    - Usar '(())' para inicio y fin
    - Usar '{}' para condicionales/decisiones
    - Usar '[]' para procesos/acciones clave
    - Evitar subprocesos
    - No añadir colores extra a los nodos
    - No usar emojis

## FORMATO DE SALIDA

El diagrama debe ser limpio, legible y seguir la sintaxis exacta de Mermaid 
y buenas prácticas de diseño de flujos

Consideraciones Adicionales

- Incluye todos los pasos críticos del proceso
- Identifica claramente los puntos de decisión
- Destaca interacciones con sistemas o herramientas
- Representa el flujo de información de principio a fin
- El diagrama debe ser tan detallado como sea necesario, pero sin perder claridad

