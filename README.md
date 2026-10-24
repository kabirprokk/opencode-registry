# OpenCode Marketplace Registry

A community registry of skills, agents, and commands for [OpenCode](https://github.com/anomalyco/opencode).

## Browse & install

Install the CLI:
```bash
npm install -g opencode-marketplace
```

Commands:
```bash
ocm list              # list all packages
ocm search <query>    # search
ocm info <name>       # details
ocm install <name>    # install to ~/.config/opencode/
ocm remove <name>     # uninstall
```

## Publish your own

1. Create a GitHub repo with your skill/agent/command (following OpenCode's format).
2. Fork this registry.
3. Add an entry to `registry.json`.
4. Open a PR.

### Entry format

```json
{
  "name": "my-skill",
  "type": "skill",
  "version": "1.0.0",
  "description": "What it does",
  "author": "your-github-username",
  "repo": "https://github.com/you/my-skill",
  "path": "skills/my-skill",
  "install": "git",
  "tags": ["tag1", "tag2"],
  "license": "MIT"
}
```

Types: `skill`, `agent`, `command`, `skill-pack`.

## License
MIT
