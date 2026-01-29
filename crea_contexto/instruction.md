---
version: 0.1.0
description: Crea un mapa de contexto a partir de archivos de texto
tags:
    - context-management
lang: es
---
Estás analizando una colección de archivos de texto para crear un mapa de contexto.

## Área de enfoque
{{focus}}

## Archivos a analizar

Los siguientes archivos han sido procesados con muestreo adaptativo:
- Archivos cortos (<100 líneas): contenido completo incluido
- Archivos medianos (100-500 líneas): primeras 80 líneas incluidas
- Archivos largos (>500 líneas): muestra distribuida en 5 secciones

{{input}}

## Tu tarea

Crear un documento markdown que:

1. Agrupe archivos por áreas temáticas (no por estructura de directorios)
2. Describa qué contiene cada archivo en 1-3 oraciones
3. Enlace archivos usando sintaxis markdown relativa: [nombre_archivo](./nombre_archivo.ext)
4. Marque vacíos de conocimiento con [specify: pregunta específica]
5. Priorice información relevante al área de enfoque

Nota: Para archivos mostrados como muestras, describe los temas generales visibles en los extractos distribuidos.

## Reglas

- Escribe en lenguaje natural, como si estuvieras informando a un colega
- Usa encabezados de sección descriptivos para organizar por área lógica
- No resumas el contenido, describe qué aborda el archivo
- Mantén el mapa escaneable en 2-3 minutos
- Enfócate únicamente en contenido relevante al área de enfoque

## Formato de salida

Markdown con secciones claras y referencias enlazadas.

