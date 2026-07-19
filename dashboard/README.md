# Dashboard Module

This directory will contain the modular Home Assistant dashboard implementation.

## Structure

```text
dashboard/
├── assets/   # Images, icons, and static visual assets.
├── cards/    # Independent dashboard cards.
├── theme/    # Theme files, CSS variables, and Card-mod foundations.
└── README.md
```

## Rules

- Do not create a single massive YAML file.
- Keep each card independent.
- Document every dependency before using it.
- Prefer reusable visual tokens over duplicated styling.
- Preserve the JARVIS-inspired dark supervision aesthetic.

## v0.1 Status

The dashboard architecture exists, but no interface has been implemented yet.
