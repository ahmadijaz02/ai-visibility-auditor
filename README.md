# AI Visibility Auditor

An open-source toolkit for auditing how well websites are understood, discovered, and cited by AI-powered search and answer engines.

## What it checks

- robots.txt and AI crawler access
- llms.txt and AI discovery files
- JSON-LD / structured data
- metadata and canonical URLs
- content structure and citability signals
- brand/entity consistency
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

## License and attribution

This repository is an adaptation of the MIT-licensed **GEO Audit / GEO Optimizer** project by its original authors. The original MIT license and required copyright notice are preserved in this repository.

Original project:
https://github.com/NadeemAhmad3/GEO_Audit

The code in this repository has been reorganized/rebranded for the **AI Visibility Auditor** project; this repository does not claim original authorship of the upstream code.
