# promptpipe

Tiny streaming CLI for OpenAI-compatible chat APIs

## Usage

```bash
chatsh explain this error < error.log
cat diff.patch | chatsh review this diff
```

## Features

- Streams tokens as they arrive
- Works with any OpenAI-compatible endpoint
- Model and system prompt via flags or env
- Reads the prompt from args or stdin

## Installation

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=sk-...
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── LICENSE
├── chatsh.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Acknowledgments

- README structure inspired by popular OSS templates
- Thanks to everyone opening issues with ideas

## License

MIT - see [LICENSE](LICENSE).
