# FreeGuard VPN - Public Releases

Public releases, AI agent skills, and installation scripts for [FreeGuard VPN](https://freeguardvpn.com).

## Install CLI

**macOS / Linux:**
```bash
curl -fsSL https://downloadcli.freeguardvpn.com/cli/install.sh | sh
```

**Windows (PowerShell):**
```powershell
irm https://downloadcli.freeguardvpn.com/cli/install.ps1 | iex
```

**macOS (Homebrew):**
```bash
brew install planetlinkinc/tap/freeguardvpn
```

## AI Agent Skill

Install the `freeguard-setup` skill to let AI agents (OpenClaw, Claude Code, Cursor, etc.) set up VPN for you:

```bash
curl -fsSL https://downloadcli.freeguardvpn.com/cli/skill.sh | sh
```

Or via OpenClaw:
```bash
clawhub install freeguard-setup
```

## Links

- [Website](https://freeguardvpn.com)
- [CLI Documentation](https://freeguardvpn.com/cli)
- [AI Agent Integration](https://freeguardvpn.com/cli/agent)
- [Homebrew Tap](https://github.com/planetlinkinc/homebrew-tap)
