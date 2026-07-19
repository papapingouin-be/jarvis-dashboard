# JARVIS Dashboard

**Version:** v0.1  
**Status:** Open source project bootstrap

JARVIS Dashboard is a Home Assistant supervision interface designed for monitoring an AI coding agent in real time. It is not intended to look or feel like a default Home Assistant dashboard. The design direction combines the operational clarity of NASA Mission Control, the observability density of Grafana, the container-focused structure of Portainer, the developer ergonomics of VSCode, the camera/system awareness of Frigate, and a subtle Iron Man JARVIS-inspired visual language.

## Vision

The dashboard should make an AI agent feel alive and observable. In less than two seconds, a user should understand:

- what Codex is currently doing;
- how long it has been running;
- which files are being modified;
- which command is executing;
- whether the system is healthy.

Data will be provided primarily through MQTT and rendered through modular Home Assistant dashboard components.

## Design Principles

- Dark, cinematic, high-contrast interface.
- Minimal text with generous spacing.
- Rounded cards and soft depth.
- Discreet motion only: no aggressive blinking.
- Every card is independent and documented.
- Architecture must remain modular and maintainable.

## Visual Palette

| Role | Color |
| --- | --- |
| Background | `#101418` |
| Card | `#181E24` |
| Blue | `#45C7FF` |
| Green | `#37D67A` |
| Orange | `#FFA940` |
| Red | `#FF4D4F` |
| Text | `#F4F7FA` |
| Accent | Cyan |

## Repository Structure

```text
.
├── dashboard/
│   ├── assets/
│   ├── cards/
│   ├── theme/
│   └── README.md
├── docs/
├── CHANGELOG.md
├── LICENSE
├── README.md
└── ROADMAP.md
```

## Version v0.1 Scope

This release only creates the initial open source project structure:

- professional project README;
- MIT license;
- roadmap;
- changelog;
- Git ignore rules;
- modular dashboard folders;
- initial dashboard documentation.

No dashboard interface is implemented in v0.1.

## Planned Home Assistant Integrations

Future versions may use the following components when they are relevant:

- Mushroom;
- Bubble Card;
- Card-mod;
- Layout-card;
- Auto-entities;
- ApexCharts;
- Markdown cards;
- Conditional cards;
- Grid and Sections layouts;
- Browser_mod if it adds meaningful value.

Dependencies will never be imposed unnecessarily. Each dependency must be documented before use.

## License

This project is released under the MIT License. See [LICENSE](LICENSE).
