# Contributing to Renovate Config

This is a personal repository containing Renovate configuration presets. While contributions are not actively sought, suggestions and improvements are welcome.

## Configuration Structure

- **`default.json`** - Main configuration preset extending all sub-presets
- **`autoMerge.json5`** - Auto-merge rules for safe dependency updates
- **`labels.json5`** - PR labeling rules based on update types and package managers
- **`semanticCommits.json5`** - Semantic commit message formatting
- **`renovate.json`** - Self-hosting configuration for this repository

## Testing Changes

Before making changes:

1. Validate JSON/JSON5 syntax
2. Check against Renovate schema
3. Test in a separate repository first

## Schema Validation

All configuration files use the official Renovate schema:
```
https://docs.renovatebot.com/renovate-schema.json
```

## Useful Links

- [Renovate Documentation](https://docs.renovatebot.com/)
- [Configuration Options](https://docs.renovatebot.com/configuration-options/)
- [Preset Templates](https://docs.renovatebot.com/config-presets/)
