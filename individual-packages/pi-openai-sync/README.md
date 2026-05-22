# @thawee/pi-openai-sync

OpenAI-compatible model sync extension for the [Pi Coding Agent](https://github.com/badlogic/pi-mono).

Auto-populate `models.json` with models from any OpenAI-compatible API (e.g. Together, DeepInfra, Hyperbolic, OpenRouter, or custom local gateways).

## Installation

```bash
# Install directly via Pi
pi install git:github.com/thawee/pi-openai-sync
```

## Commands

```bash
# Sync with URL (defaults to 'openai' provider)
/openai-sync https://api.deepinfra.com/v1

# Sync with API key
/openai-sync https://api.deepinfra.com/v1 sk-your-key

# Sync to a custom provider target name
/openai-sync https://api.together.xyz/v1 sk-your-key together
```

## Features

- Queries OpenAI-compatible `/v1/models` (or custom `/models`) endpoint.
- Support optional API bearer token authentication.
- Automatically creates new provider targets in `models.json` or updates existing ones.
- Preserves existing custom provider properties (apiKey, baseUrls, compat configs).
- Auto-detects reasoning-capable models (e.g. `deepseek-r1`, `o1-mini`).
- Auto-detects model families (e.g. `llama`, `qwen`, `deepseek`).
- Safe atomic file I/O operations on `models.json`.
- Registered as both `/openai-sync` command and `openai_sync` tool.

## Links

- [GitHub Repository](https://github.com/thawee/pi-openai-sync)

## License

- MIT
