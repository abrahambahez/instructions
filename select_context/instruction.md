---
version: 0.1.0
description: File-based context management selector
tags:
    - context-management
lang: en
---
## PORPOUSE
You are analyzing a context file to determine which linked resources are needed.

Context file: {{input|context}}

Instruction intent: {{intent}}

## TASK

1. Analyze the context structure and links
2. Determine which linked files are relevant for the given intent
3. Output ONLY the file paths, one per line, no other text

Consider:
- What information does this instruction need?
- Which linked resources contain that information?
- What can be safely omitted?

Output format (CRITICAL - output ONLY this, nothing else):
path/to/file1.md
path/to/file2.csv
