# Skills Dossiers (LaTeX)

This repository contains structured, LaTeX-based study dossiers for technical skills (e.g., SQL, Angular, Spring).
Each skill is written as a single compiled document (PDF) but maintained as multiple LaTeX section files for readability and version control.

## Repository structure

- `latex/template/`  
  Shared LaTeX preamble and macros used across dossiers.
- `<skill>/main.tex`  
  The main entry point for compiling the skill dossier.
- `<skill>/sections/`  
  Section files included by `main.tex`.
- `<skill>/assets/`  
  Images and other resources (if needed).

Example:
- `sql/main.tex`
- `sql/sections/01-scope.tex`
- `sql/sections/02-skill-ladder.tex`
- `sql/sections/03-concept-map.tex`

## How to build (local)

### Requirements
- A LaTeX distribution:
    - macOS: MacTeX / TeX Live
    - Windows: MiKTeX
    - Linux: TeX Live

### Compile a dossier
From the repository root:

```bash
cd sql
pdflatex main.tex
pdflatex main.tex
```

(Second run is for the table of contents.)

## Notes
- Generated PDFs and LaTeX build artifacts are intentionally not committed.
- CI compilation can be added later for practice (GitHub Actions / GitLab CI).