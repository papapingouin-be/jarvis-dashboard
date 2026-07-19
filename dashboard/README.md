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

## v0.3 Status

The dashboard now includes one screen only: `views/mission-control.yaml`. It is designed as the official Mission Control screenshot with three responsive columns, system cards, a central mission card, terminal console, event timeline, and daily summary.


## v0.3 Dependencies

- `layout-card`: required only for the Mission Control screen to preserve the 25% / 50% / 25% desktop proportions and responsive single-column fallback.
- `card-mod`: required for the polished dark cards, glows, status indicators, progress animation, and terminal reveal effect.
