# Changelog

All notable changes to the Pi OpenAI Sync extension (`@thawee/pi-openai-sync`) will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-05-22

### Added

- Initial release of the Pi OpenAI Sync extension.
- `/openai-sync` slash command for manual model synchronization.
- `openai_sync` tool for autonomous model synchronization by the agent.
- Support for any OpenAI-compatible `/v1/models` endpoint.
- Automatic detection of reasoning-capable models (e.g., DeepSeek-R1, OpenAI o1).
- Automatic model family classification for optimal formatting.
- Atomic configuration updates to `models.json`.
- Support for custom provider target names.
