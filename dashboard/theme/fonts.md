# Jarvis Dark typography

Jarvis Dark uses a restrained, technical typography stack that remains compatible
with default Home Assistant installations.

## Recommended stack

- **Primary UI:** `Inter`, then `Roboto`, then system UI fallbacks.
- **Monospace/data:** `JetBrains Mono`, then `Roboto Mono`, then system monospace fallbacks.

## Installation options

1. Use the built-in fallbacks only. Home Assistant already ships with Roboto in
   most installations, so the theme remains usable without extra resources.
2. Optionally install Inter and JetBrains Mono locally through `www/fonts/` and
   reference them with a Home Assistant frontend resource or a custom CSS loader.
3. Avoid loading many font weights. The design system only needs 400, 500, 600,
   and 700.

## Usage rules

- Titles use weight 700 with slight positive letter spacing.
- Labels and badges use uppercase text with wider letter spacing.
- Body text uses weight 400 or 500 for readability.
- Numeric telemetry may use the monospace stack when alignment matters.
