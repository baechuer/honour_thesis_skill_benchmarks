---
name: metrics-root-cause-diagnoser
description: Diagnoses likely causes behind an operational regression or incident by connecting multiple metrics and service signals into a plausible explanation.
---

# Metrics Root Cause Diagnoser

Builds a likely-cause explanation from multiple operational signals.

## Use when

- The user wants help understanding what is driving a regression, outage, or performance problem.
- The input includes several related metrics or observations rather than one isolated chart.
- The output should connect signals into a plausible operational explanation.

## Workflow

1. Identify the main regression or incident symptom.
2. Look for supporting and contradicting signals across latency, errors, traffic, saturation, or dependency indicators.
3. Form the most plausible cause hypothesis or ranked hypotheses.
4. Note what evidence is missing or ambiguous.
5. Return a compact diagnostic explanation with next checks.

## Writing rules

- Prefer plausible causal structure over a list of disconnected observations.
- Distinguish strong evidence from speculation.
- Include what would confirm or falsify the leading hypothesis.
- Return only the diagnosis unless the user asks for more.

## Output pattern

Use this shape unless the user asks for something else:

- Main symptom
- Likely cause or causes
- Supporting signals
- Contradicting or missing signals
- Next checks

For worked examples, see `examples.md`.
