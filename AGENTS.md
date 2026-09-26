# AGENTS.md - Guide for AI Agents

This file provides context and guidance for AI agents (like Claude Code) working on this project.

## Project Overview

**ai-notebooks** is a collection of Jupyter notebooks teaching AI fundamentals through hands-on tutorials. The project covers Machine Learning, Deep Learning, and Reinforcement Learning with a focus on running AI locally.

- **Python**: >=3.11
- **Package manager**: [uv](https://github.com/astral-sh/uv) (not pip/poetry)
- **Runtime**: Jupyter notebooks (`.ipynb`) are the primary artifact
- **Code style**: [Ruff](https://docs.astral.sh/ruff/) (target: py312)

## Directory Structure

```
ai-notebooks/
├── 00-ML/                    # Machine Learning tutorials
│   └── 00-regression/        # Supervised learning & linear regression
├── 01-DL/                    # Deep Learning tutorials
│   └── 00-data-extraction/   # Docling + NuExtract for PDF/image parsing
├── pyproject.toml            # Project config & dependencies
├── uv.lock                   # Deterministic dependency lock file
├── README.md                 # User-facing documentation
└── CONTRIBUTING.md           # Community contribution guidelines
```

## Dependencies

Managed via `uv`. Key dependencies:

| Category     | Packages                                              |
|------------- |-------------------------------------------------------|
| Core ML      | scikit-learn, numpy, pandas, scipy                    |
| Visualization| matplotlib, seaborn                                   |
| Deep Learning| torch, torchvision                                    |
| Data parsing | docling[vlm], pydantic                                |
| Datasets     | kaggle, hf-xet                                        |
| Dev          | ruff                                                  |

Install with: `uv sync`

## Working with Notebooks

- Notebooks are the main deliverable. When editing `.ipynb` files, treat them as code — verify cells run end-to-end and don't break existing cell outputs.
- The notebooks reference Kaggle datasets; a Kaggle API key (`kaggle.json`) is required to fetch data.
- Python 3.12+ conventions apply (ruff target-version).

## Code Style

Ruff enforces:

- 100-char line limit
- Double quotes, space indentation
- Import sorting (isort)
- Auto-upgrade to newer syntax
- Ignores E501 (let the formatter handle it)

Lint/format: `ruff check .` / `ruff format .`

## Contribution Rules

- All feedback goes through [GitHub Discussions](https://github.com/anima-kit/ai-notebooks/discussions).
- No Issues or Pull Requests are accepted for this repo.
- Security vulnerabilities: follow [SECURITY.md](SECURITY.md) and use GitHub's Private Vulnerability Reporting.
- See [CONTRIBUTING.md](CONTRIBUTING.md) for participation guidelines.

## Agent-Specific Notes

- **Always use `uv`** for dependency management, never pip directly.
- **Activate the venv** before running notebooks: `.venv/Scripts/activate` (Windows) or `source .venv/bin/activate` (Linux/Mac).
- When suggesting changes to notebooks, keep explanations beginner-friendly — this is an educational project.
- Link related tutorials in [anima-kit/tutorials](https://anima-kit.github.io/tutorials/) when relevant.
