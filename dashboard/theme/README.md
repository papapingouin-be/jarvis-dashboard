# Jarvis Dark theme (v0.2)

This folder contains only the visual identity for the project. It does not define
business cards, dashboards, MQTT entities, automations, or domain-specific views.

## Files

- `variables.yaml` — design tokens for palette, spacing, radii, typography,
  shadows, animations, and responsive layout rules.
- `theme.yaml` — Home Assistant compatible theme named **Jarvis Dark**.
- `card-mod.yaml` — reusable card-mod style snippets for cards, titles, chips,
  Mushroom cards, Markdown, entities, and separators.
- `fonts.md` — typography guidance and optional font installation notes.

## Dependencies

Required:

- Home Assistant with YAML themes enabled.

Optional but recommended:

- [`card-mod`](https://github.com/thomasloven/lovelace-card-mod) for applying the
  shared card styling snippets.
- Mushroom cards if future dashboard cards use Mushroom components. The design
  system includes Mushroom variables but does not create any Mushroom cards.
- Inter and JetBrains Mono fonts if you want the exact recommended typography.

## Install the Home Assistant theme

1. Copy `theme.yaml` into your Home Assistant themes directory, for example:
   `config/themes/jarvis-dark.yaml`.
2. Ensure themes are enabled in `configuration.yaml`:

   ```yaml
   frontend:
     themes: !include_dir_merge_named themes
   ```

3. Restart Home Assistant or reload themes from Developer Tools.

## Activate Jarvis Dark

1. Open your Home Assistant user profile.
2. In **Theme**, select **Jarvis Dark**.
3. Refresh the browser if the theme is not immediately applied.

## Use card-mod snippets

Copy the relevant snippets from `card-mod.yaml` into future Lovelace cards or
include them through your preferred YAML structure. The snippets are intentionally
generic and should be reused as the baseline for all future cards.

## Responsive guidance

- Desktop: generous spacing, 22px card padding, and subtle hover lift.
- Tablet: slightly reduced spacing and 18px card padding.
- Mobile: compact spacing, 16px card padding, and hover lift disabled to keep
  touch interactions stable.

## Animation policy

Animations are discreet and short. No blinking, flashing, or aggressive looping
motion is used in this design system.
