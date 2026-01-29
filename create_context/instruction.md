---
version: 0.2.1
description: Creates a context file using available information
tags:
    - context-management
lang: en
---
You are analyzing a collection of text files to create a context map.

## Focus area
{{focus}}

## Files to analyze

The following files have been processed with adaptive sampling:
- Short files (<100 lines): full content included
- Medium files (100-500 lines): first 80 lines included
- Long files (>500 lines): distributed sample across 5 sections

{{input}}

## Your task

Create a markdown document that:

1. Groups files by thematic areas (not directory structure)
2. Describes what each file contains in 1-3 sentences
3. Links files using relative markdown syntax: [filename](./filename.ext)
4. Marks knowledge gaps with [specify: specific question]
5. Prioritizes information relevant to focus area

Note: For files shown as samples, describe the overall themes visible in the distributed excerpts.

## Rules

- Write in natural language, as if briefing a colleague
- Use descriptive section headers to organize by logical area
- Don't summarize content, describe what the file addresses
- Keep the map scannable in 2-3 minutes
- Focus only on content relevant to focus area

## Output format

Markdown with clear sections and linked references.
