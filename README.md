# White — Light Theme for Hermes Dashboard

[![GitHub](https://img.shields.io/badge/repo-hermes--white--theme-blue)](https://github.com/orlandoburli/hermes-white-theme)

A clean white/light theme for the [Hermes Agent](https://hermes-agent.nousresearch.com) web dashboard. Features an off-white background with dark charcoal text, Inter sans-serif, and JetBrains Mono for code.

## Preview

- **Background:** `#f5f0eb` (warm off-white)
- **Text:** `#1a1a2e` (dark charcoal)
- **Accent:** Warm glow with reduced noise opacity
- **Fonts:** Inter (UI) + JetBrains Mono (code)
- **Backdrop:** Screen blend mode for light backgrounds

## Installation

1. Copy `white.yaml` to your Hermes dashboard themes directory:

   ```bash
   mkdir -p ~/.hermes/dashboard-themes
   cp white.yaml ~/.hermes/dashboard-themes/
   ```

2. Restart the Hermes dashboard:

   ```bash
   hermes dashboard --stop
   hermes dashboard
   ```

3. Open http://localhost:9119 and select **White** from the theme picker.

## How it works

Hermes Agent's web dashboard automatically discovers user themes in `~/.hermes/dashboard-themes/*.yaml`. The backend reads the YAML, normalizes it, and serves the full definition to the frontend — no code changes needed.

Your theme is stored outside the Hermes installation directory, so it survives `hermes update`.

## Requirements

- Hermes Agent v0.14.0+
- Node 20.19+ or 22.12+ (for dashboard builds)

## License

MIT
