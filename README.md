# 🤖 Personal Renovate Configuration

[![Renovate](https://github.com/vrozaksen/renovate-config/actions/workflows/renovate.yaml/badge.svg)](https://github.com/vrozaksen/renovate-config/actions/workflows/renovate.yaml)
[![Label Sync](https://github.com/vrozaksen/renovate-config/actions/workflows/label-sync.yaml/badge.svg)](https://github.com/vrozaksen/renovate-config/actions/workflows/label-sync.yaml)
[![Last Commit](https://img.shields.io/github/last-commit/vrozaksen/renovate-config)](https://github.com/vrozaksen/renovate-config/commits/main)
[![License](https://img.shields.io/github/license/vrozaksen/renovate-config)](LICENSE)

My personal Renovate configuration presets for automated dependency management across my projects.

## Configuration Files

- **`default.json`** - Main preset that extends all other configurations
- **`autoMerge.json5`** - Auto-merge rules for trusted dependencies
- **`labels.json5`** - Automatic PR labeling by update type and package manager  
- **`semanticCommits.json5`** - Semantic commit message formatting
- **`renovate.json`** - Self-hosting configuration for this repository

## Key Features

- **Smart Auto-merging**: Trusted GitHub Actions merge immediately, others after 3 days
- **Semantic Commits**: Consistent `feat(scope):`, `fix(scope):`, `chore(scope):` formatting
- **Comprehensive Labeling**: Automatic categorization by update type and technology
- **Security**: Pinned GitHub Action digests and careful auto-merge rules
- **Timezone**: Configured for Europe/Warsaw

## Usage in My Projects

Add to `renovate.json` in any repository:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>vrozaksen/renovate-config"]
}
```

## Automated Workflows

- **Renovate**: Runs hourly to check for dependency updates
- **Label Sync**: Daily synchronization of repository labels
