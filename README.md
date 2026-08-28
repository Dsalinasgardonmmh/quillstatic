# quillstatic

Static blog generator: markdown in, tidy HTML out

Side project, maintained when I have time.

## Examples

```bash
mkdir posts && echo '# hello' > posts/first.md
python build.py
# site lands in dist/
```

## What it does

- Markdown posts with fenced code and tables
- RSS feed generation
- Index page with post list by date
- Single template, plain str.format, no Jinja

## Install

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── SECURITY.md
├── build.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
