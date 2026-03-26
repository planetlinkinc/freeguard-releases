# FreeGuard VPN CLI

Official binary releases, AI agent skills, and installation scripts for [FreeGuard VPN](https://freeguardvpn.com).

> **Developed by [Planetlink Inc.](https://freeguardvpn.com)** — the CLI source code is proprietary.

## Install

### Option 1 (Recommended): Homebrew

```bash
brew install planetlinkinc/tap/freeguardvpn
```

Signed formula, checksum-verified, auto-updates. Formula source: [planetlinkinc/homebrew-tap](https://github.com/planetlinkinc/homebrew-tap)

### Option 2: GitHub Release

Download pre-built binaries from the [Releases](https://github.com/planetlinkinc/freeguard-releases/releases/latest) page.

Each release includes `checksums.txt` (SHA256) for verification:

```bash
# Download binary + checksums
curl -fsSL -L https://github.com/planetlinkinc/freeguard-releases/releases/latest/download/freeguard-darwin-arm64.tar.gz -o freeguard.tar.gz
curl -fsSL -L https://github.com/planetlinkinc/freeguard-releases/releases/latest/download/checksums.txt -o checksums.txt

# Verify checksum
shasum -a 256 -c checksums.txt --ignore-missing

# Extract and install
tar xzf freeguard.tar.gz
sudo mv freeguard /usr/local/bin/
```

### Option 3: Install script

```bash
# macOS / Linux
curl -fsSL https://downloadcli.freeguardvpn.com/cli/install.sh | sh

# Windows (PowerShell)
irm https://downloadcli.freeguardvpn.com/cli/install.ps1 | iex
```

## Platforms

| File | Platform |
|------|----------|
| `freeguard-darwin-arm64.tar.gz` | macOS (Apple Silicon) |
| `freeguard-darwin-amd64.tar.gz` | macOS (Intel) |
| `freeguard-linux-amd64.tar.gz` | Linux (x64) |
| `freeguard-linux-arm64.tar.gz` | Linux (ARM64) |
| `freeguard-windows-amd64.zip` | Windows (x64) |

## AI Agent Skill

The `freeguard-setup` skill lets AI agents (Claude Code, Cursor, OpenClaw, etc.) guide users through VPN setup:

```bash
clawhub install freeguard-setup
```

## Links

- [Website](https://freeguardvpn.com)
- [Homebrew Tap](https://github.com/planetlinkinc/homebrew-tap)
- [Latest Release](https://github.com/planetlinkinc/freeguard-releases/releases/latest)
