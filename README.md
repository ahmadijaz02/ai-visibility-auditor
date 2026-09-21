# AI Visibility Auditor.

An open-source toolkit for auditing how well websites are understood, discovered, and cited by AI-powered search and answer engines.

## What it checks

- robots.txt and AI crawler access
- llms.txt and AI discovery files
- JSON-LD / structured data
- metadata and canonical URLs
- content structure and citability signals
- brand and entity consistency
- AI crawler and access readiness
- citation and visibility signals
- actionable recommendations with machine-readable output

## Quick start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -e .
```

Run an audit:

```bash
geo audit --url https://example.com
```

JSON output:

```bash
geo audit --url https://example.com --format json
```

## Project structure

```text
src/geo_optimizer/   Core audit engine and CLI
tests/               Automated tests
frontend/            Optional Astro frontend
docs/                Project documentation
```

## Development

```bash
pip install -e ".[dev]"
pytest
ruff check .
```

## Features

- Website-level AI visibility auditing
- AI crawler and robots.txt analysis
- llms.txt validation
- Structured data and schema analysis
- Metadata and content-quality checks
- Brand/entity and citation-signal analysis
- Machine-readable JSON reports
- CLI workflow for local and CI usage

## License

This project is released under the MIT License. See [LICENSE](LICENSE) for the full license text.

The project is based on and adapted from the GEO Audit codebase, with the implementation organized and rebranded as **AI Visibility Auditor**.
