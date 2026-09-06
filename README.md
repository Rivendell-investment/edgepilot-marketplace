# EdgePilot

Official self-hosted plugin marketplace for EdgePilot Live and Research.

This branch is `feat/refactoring`. Marketplace ID: `edgepilot`.

## Codex

```bash
codex plugin marketplace add Rivendell-investment/dgepilot-marketplace --ref feat/refactoring
codex plugin add edgepilot@edgepilot
codex plugin add edgepilot-research@edgepilot
```

## Claude Code

```bash
claude plugin marketplace add Rivendell-investment/dgepilot-marketplace@feat/refactoring
claude plugin install edgepilot@edgepilot
claude plugin install edgepilot-research@edgepilot
```

Install either product or both. Node.js must be available to the host. Reload plugins or start a new session after installation. Plugin installation does not mean Runtime is running: ask to start EdgePilot, then open its Dashboard. The production Runtime currently supports macOS arm64. Live login is Dashboard-only; Research needs no account.

Branches share one marketplace identity; configure only one branch at a time. Do not enable another marketplace's copy of the same product alongside this one.

## Release ownership

Generated from audited production plugin ZIPs through the source repository's `./build.sh marketplace-sync` command. `release.json` records input hashes and generated plugin hashes. Runtime downloads remain on each product's public channel. No credentials, Python, Runtime or user state are stored here.
