# Skill Benchmark

This folder contains the working benchmark materials for my honours thesis on skill representation and retrieval for personal LLM agents.

The benchmark is grounded in recurring personal workflows rather than a random collection of tasks. The current skill families were chosen because they reflect realistic day-to-day knowledge work, including reading, writing, replying to messages, planning, handling documents, analysing spreadsheets, and interpreting operational metrics. These are the kinds of tasks that a personal agent could reasonably accumulate over time through custom skills or prebuilt skill libraries.

The central research problem is not simply whether skills are useful. It is whether an agent can select the correct skill when several skills look similar at the description level but differ procedurally in their inputs, outputs, workflow steps, preconditions, or success criteria.

This benchmark is therefore being developed in two layers:

1. A confusable core of carefully authored skills and test cases, where the procedural difference is clear and the gold skill can be annotated reliably.
2. A larger background library of additional skills used to create retrieval pressure, context growth, and more realistic selection conditions.

Public skill libraries are used as realism seeds for naming conventions, metadata style, and workflow patterns. However, the final benchmark skills are being authored and normalized here so that the resulting clusters have controlled semantic confusability and stable gold labels.

## Current folder structure

- `skills/`
  - one folder per benchmark skill
  - each skill can later contain `SKILL.md`, metadata, examples, or supporting files
- `clusters/`
  - cluster definitions describing which skills are confusable and why
- `prompts/`
  - benchmark prompts, candidate skills, and gold labels
- `notes/`
  - design notes, rationale, and benchmark decisions

## Current candidate skill families

- reading / research
- news / monitoring
- reply / messaging
- email / communication
- planning / meetings
- documents / files
- data / spreadsheet
- metrics / observability

These categories may be refined as the benchmark becomes more grounded in my own actual workflows and as confusable cases are tested against candidate skill descriptions.
