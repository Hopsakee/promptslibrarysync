Explore this codebase and create two Mermaid diagrams with documentation:

**1. Architecture Diagram (flowchart TB)**
- Read every module in the main package directory to understand what each does
- Read pyproject.toml, README, and any design/PRD docs for context
- Classify each module: 🟢 Done (real logic), 🟡 Partial/Broken (incomplete, broken imports, TODOs), 🔴 Stub (placeholder only)
- Create a top-to-bottom flowchart with:
  - External systems at the top (files, APIs, databases)
  - Modules grouped into subgraphs by layer (ingestion, storage, domain, web/API, entry)
  - Arrows showing data flow with labels
  - Color-coded status using classDef:
    - done: fill:#1a5c1a,stroke:#2ecc71,color:#fff
    - partial: fill:#7d5a00,stroke:#f39c12,color:#fff
    - stub: fill:#7a1a1a,stroke:#e74c3c,color:#fff
    - ext: fill:#1a3a5c,stroke:#3498db,color:#fff

**2. Data Model Diagram (erDiagram)** — if the project has database models/dataclasses
- Show all entities with fields, types, PK/FK/UK annotations
- Show relationships with correct cardinality
- Include entities referenced in code but not yet defined as models

**Output**: Create a `docs_md/` folder with two markdown files:
- `docs_md/architecture.md`: Diagram + prose explaining each layer, a module status table, key issues found, and recommended next steps
- `docs_md/datamodel.md`: ER diagram + entity descriptions, relationship tables (implemented vs planned), and known schema issues

Use ```mermaid syntax (no curly braces) in the markdown files for GitHub compatibility.

Render both diagrams inline so I can see them now.

Also create Jupyter notebooks that contain the same content:
- All prose in markdown cells
- Mermaid diagrams in markdown cells using ```{mermaid} syntax (for quarto rendering)
- A final code cell that reads the notebook's own markdown cells and writes to docs_md/,
  converting ```{mermaid} to ```mermaid for GitHub compatibility
- This keeps notebooks and markdown files in sync: run the notebook to regenerate the markdown
