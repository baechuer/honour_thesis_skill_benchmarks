---
name: reply-drafter
description: Drafts a reply message or email from conversation context. Use when the user needs a fresh reply written from the source message and does not already have a usable draft.
---

# Reply Drafter

Writes a sendable reply from the source message and the user's goal.

## Use when

- The user wants to reply to an email, chat message, or thread.
- The user provides source context but not a usable reply draft.
- The main task is to produce a new response that can be sent with light editing.

## Not for

- Polishing an existing reply draft.
- Summarizing a thread without writing a reply.
- Extracting only tasks or deadlines.
- Recipient-specific cases where a more specialized reply skill is clearly a better fit.

## Workflow

1. Identify what the sender is asking, implying, or expecting.
2. Infer the user's likely response goal from the prompt and context.
3. Draft a reply that addresses the important points directly.
4. Preserve key facts, dates, and commitments from the context.
5. Keep the message clear, sendable, and appropriately concise.

## Writing rules

- Do not invent facts, promises, or deadlines not supported by the context.
- Prefer a direct, professional tone unless the context clearly suggests otherwise.
- If context is missing, ask for clarification inside the draft rather than hallucinating details.
- Return only the reply unless the user asks for alternatives or explanation.
