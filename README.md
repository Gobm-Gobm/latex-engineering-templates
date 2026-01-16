LaTeX Engineering Templates

Reusable LaTeX templates for professional engineering documentation.

Purpose

Create consistent, consultant-grade engineering documents

Provide a stable, reusable LaTeX report layout (header, footer, margins)

Separate layout, content, and company-specific data

Serve as a personal documentation standard for consulting work

Form a solid base for future automation (Python → LaTeX)

This repository intentionally focuses on clarity and stability over flexibility.
Abstractions are only introduced when there is a real need.

Current Status

Version: v1.0.0

Stable report layout using geometry and fancyhdr

Header includes:

Company logo (left)

Document title, subtitle, and project (center)

Revision metadata (right, visually de-emphasised)

Footer includes:

Company identity emphasized

Contact details greyed out

Clear page numbering

Designed for A4 print output

This version is considered a solid baseline.

Repository Structure
latex-engineering-templates/
├─ templates/
│  ├─ report/
│  │  ├─ preamble.tex   # Packages and global setup
│  │  ├─ layout.tex     # Geometry and header/footer layout
│  │  └─ macros.tex     # Document, header, and footer macros
│  │
│  ├─ companies/
│  │  ├─ aconsult_uk.tex
│  │  └─ aconsult_dk.tex
│  │
│  └─ assets/
│     └─ aconsult_logo.png
│
├─ examples/
│  └─ drawing-code-description/
│
├─ docs/
│  └─ design-decisions.md
│
└─ README.md

Design Principles

Stability first – avoid layout hacks and fragile constructs

Explicit dependencies – required packages are loaded directly

Minimal abstraction – no unused style layers or premature structure

Print-focused – layouts are optimised for PDF and A4 output

Incremental evolution – changes are made in small, reversible steps

How to Use

Copy an example from examples/

Adjust document metadata in main.tex

Select the appropriate company file

Compile with:

pdflatex main.tex


Run twice for correct page numbering.

Future Direction (Not Implemented Yet)

Title page with full QA / revision table

Conditional display of metadata fields

Multiple document types (memo, specification)

Automated document generation via Python

These will be considered only when needed.