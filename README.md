# Dakera APT Repository

APT/deb package repository for [Dakera AI](https://dakera.ai) tools.

## Install

```bash
# Add Dakera GPG key
curl -fsSL https://dakera-ai.github.io/apt-repo/KEY.gpg | sudo gpg --dearmor -o /usr/share/keyrings/dakera.gpg

# Add repository
echo "deb [signed-by=/usr/share/keyrings/dakera.gpg] https://dakera-ai.github.io/apt-repo stable main" \
  | sudo tee /etc/apt/sources.list.d/dakera.list

# Install dk CLI
sudo apt update && sudo apt install dk
```

## Packages

| Package | Description |
|---------|-------------|
| `dk` | Dakera CLI — manage AI agent memory from the command line |

## Updates

Packages are automatically published when a new version of dakera-cli is released.
