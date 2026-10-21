# Task: Design Process Flow

## Goal
Convert the approved Clarified Requirement and approved user stories
into a single Mermaid flowchart representing the end-to-end process.

## Steps
1. Use the "Steps (in order)" and "Decision points" from the Clarified
   Requirement as your backbone.
2. Cross-check against the approved user stories — each story should
   be traceable to one or more nodes/branches in the diagram.
3. Follow the shared syntax rules in
   `.github/prompts/mermaid-flow-conventions.prompt.md` (node types,
   labeling, start/end requirements).
4. Make sure every decision point has clearly labeled branches, and
   every path reaches an End node.

## Output format (Markdown)
1. A one-line summary of what the diagram represents.
2. The Mermaid flowchart, in a fenced ```mermaid code block.
3. A short bullet list mapping each user story to its corresponding
   node(s)/branch(es) in the diagram.