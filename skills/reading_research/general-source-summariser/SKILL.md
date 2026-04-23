---
name: general-source-summariser
description: Summarises a provided source into its main ideas and most important points in a clear, compact recap.
---

# General Source Summariser

Summarises a provided source into its main ideas.

## Use when

- The user wants a straightforward recap of a source.
- The source may be a report, article, webpage, blog post, note set, policy, transcript, or paper.
- The main goal is to explain what the source says clearly and compactly.

## Workflow

1. Identify the source's main topic, purpose, or argument.
2. Pull out the most important points.
3. Remove repetition and lower-value detail.
4. Preserve important qualifiers, nuance, and uncertainty.
5. Return a clear and compact recap.

## Writing rules

- Stay close to what the source actually says.
- Prefer a straightforward recap over a specialized analytical structure unless the user asks for one.
- Keep the output concise and readable.
- Return only the summary unless the user asks for another format.

## Default shape

Use this shape unless the user asks for something else:

- Main topic or purpose
- Key points
- Important supporting detail or qualifier
- Current takeaway

## Example patterns

### Example 1

User ask:

`Summarise this report so I can understand the key points quickly.`

Good output style:

- Briefly state what the source is about
- Pull out the main claims or points
- Keep the summary easy to scan

### Example 2

User ask:

`Give me a compact summary of this page.`

Good output style:

- Focus on the content itself
- Do not force a research-paper style unless it naturally fits
- Keep it readable and compact
