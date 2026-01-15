# Design Decisions – LaTeX Engineering Templates

## Philosophy
- Structure over styling
- Templates enforce layout, not content
- Documents should be readable and automatable

## Separation of concerns
- Layout: `layout.tex`
- Styling: `styles/`
- Content: example-specific files
- Logic/macros: `macros.tex`

## Open questions
- How revision history should be handled
- Mandatory vs optional metadata
- When to introduce Python-generated content
