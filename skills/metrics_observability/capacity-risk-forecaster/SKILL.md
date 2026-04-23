---
name: capacity-risk-forecaster
description: Estimates near-term capacity risk from load, saturation, queueing, and headroom signals, highlighting likely bottlenecks and pressure trends.
---

# Capacity Risk Forecaster

Estimates near-term capacity risk from operational signals.

## Use when

- The user wants to know whether a system is likely to run into saturation or capacity pressure.
- The input includes utilization, throughput, queue depth, concurrency, memory, CPU, or similar load indicators.
- The output should focus on future operational risk rather than only current status.

## Workflow

1. Identify the main load and saturation indicators in the input.
2. Look for rising pressure, shrinking headroom, or coupling between demand and queueing.
3. Distinguish immediate saturation from near-term risk buildup.
4. Highlight the most plausible bottleneck or constraint.
5. Return a short capacity-risk forecast with uncertainty noted where needed.

## Writing rules

- Emphasize forward-looking operational risk.
- Prefer plausible bottlenecks over generic caution.
- Preserve uncertainty when trend history is too short or incomplete.
- Return only the forecast unless the user asks for more.

## Output pattern

Use this shape unless the user asks for something else:

- Capacity risk level
- Leading signals
- Likely bottleneck or constraint
- What to watch next

For worked examples, see `examples.md`.
