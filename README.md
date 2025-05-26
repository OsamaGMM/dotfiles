# Dotfiles Managed with chezmoi

This repo uses [chezmoi](https://www.chezmoi.io) to manage dotfiles across machines.

---

## Setup on a New Machine

1. **Install chezmoi**

```bash
# macOS (with Homebrew)
brew install chezmoi

chezmoi init https://github.com/OsamaGMM/dotfiles --apply


# Add a file to chezmoi management
chezmoi add <path-to-file>

chezmoi add ~/.zshrc

chezmoi edit <path-to-file>

chezmoi edit ~/.zshrc

chezmoi apply

chezmoi diff          # see what's changed
chezmoi apply         # apply changes to actual files
chezmoi git add -u    # stage the updated files
chezmoi git commit -m "Update"
chezmoi git push      # push to GitHub
```

Additional Tips
Avoid editing config files directly; always use config edit.

To view differences before applying, use config diff.
