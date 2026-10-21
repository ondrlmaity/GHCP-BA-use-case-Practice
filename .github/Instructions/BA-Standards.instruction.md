---
applyTo: "**"
---

# Shared BA Standards

These standards apply across all BA agents in this workflow (Requirement
Analyzer, Story Writer, Process Flow Designer, Flow Reviewer). Agents
should follow these rules whenever relevant to their task.

## Tone
- Business-friendly language. Avoid technical jargon unless the
  stakeholder requirement itself used it first.
- Be concise and structured — prefer bullet points and short sections
  over long paragraphs.

## User story standards (INVEST)
Every user story must satisfy:
- **Independent** — deliverable without depending on other stories.
- **Negotiable** — a conversation starter, not a rigid contract.
- **Valuable** — delivers clear value to a user or the business.
- **Estimable** — scoped enough to roughly size effort.
- **Small** — fits within a single sprint.
- **Testable** — has clear, verifiable acceptance criteria.

Standard format:
> **As a** [persona], **I want** [goal], **so that** [benefit].

## Acceptance criteria standard (Gherkin)
Acceptance criteria must use Given/When/Then syntax and cover:
- Happy path (main success scenario)
- At least one alternate/edge case
- At least one negative/error case (where applicable)

## Honesty about assumptions
- Never invent business rules silently. If information is missing,
  either ask a clarifying question or explicitly label it as an
  "Assumption" in the output.
