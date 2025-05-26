# Dotfiles Managed with chezmoi

This repo uses [chezmoi](https://www.chezmoi.io) to manage dotfiles across machines.

---

## Setup on a New Machine

1. **Install chezmoi**

```bash
# macOS (with Homebrew)
brew install chezmoi

config init yourusername --apply


# Add a file to chezmoi management
config add <path-to-file>

config add ~/.zshrc

config edit <path-to-file>

config edit ~/.zshrc

config apply
```

Additional Tips
Avoid editing config files directly; always use config edit.

To view differences before applying, use config diff.

# New Machine
```bash
brew install chezmoi

# Then  we do

chezmoi init https://github.com/OsamaGMM/dotfiles --apply
```
