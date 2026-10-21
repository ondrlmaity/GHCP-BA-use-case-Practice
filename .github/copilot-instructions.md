# Repository Context

This repository contains a multi-agent Business Analysis (BA) workflow
that turns a raw stakeholder requirement into reviewed user stories and
a Mermaid process flow diagram.

## Structure
- `input/` — raw stakeholder requirement file(s) (e.g.,
  `stakeholder-requirement.txt`).
- `output/` — generated artifacts; the Orchestrator writes
  `user-stories.md` and `process-flow.md` here.
- `.github/agents/` — individual agent personas (Requirement Analyzer,
  Story Writer, Process Flow Designer, Flow Reviewer, and the
  Orchestrator that coordinates them).
- `.github/prompts/` — reusable task-logic prompt files used by one or
  more agents.
- `.github/instructions/` — shared domain standards (e.g., INVEST,
  Gherkin, Mermaid conventions) referenced across multiple agents/prompts.

## How to run the workflow
To run the full pipeline, invoke `@orchestrator`. It will read the
requirement from `input/stakeholder-requirement.txt`, call each
specialist agent in sequence, and pause at human approval checkpoints.
If `input/stakeholder-requirement.txt` is missing or empty, stop and ask
the user to provide the requirement before proceeding. If multiple
requirement files exist in `input/`, ask the user which one to process.
Do not invoke the specialist agents directly unless you specifically
want to test one in isolation — the Orchestrator manages the correct
sequence and hand-offs.

## General conventions
- All generated artifacts (user stories, review notes, diagrams) must be
  written as `.md` files; Mermaid diagrams must be embedded in Markdown
  using ```mermaid fenced code blocks, not saved as standalone `.mmd`
  files.
- Keep language business-friendly; avoid unexplained technical jargon.