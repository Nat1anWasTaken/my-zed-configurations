# My Zed Configuration

## Overview
- This folder is your Zed editor config: `~/.config/zed`.
- Zed automatically reads `settings.json`, `keymap.json`, and any themes/snippets under this directory.

## What's Included
- `settings.json` — editor, UI, languages, tools configuration.
- `keymap.json` — custom keybindings.
- `themes/` — custom color themes (if any).

## Apply This Configuration
1. Close Zed if it’s open.
2. Backup your current config (recommended):

   macOS/Linux:
   ```bash
   mv ~/.config/zed ~/.config/zed.backup-"$(date +%Y%m%d-%H%M%S)"
   ```

3. Install these config files:
   - Clone this repo directly into `~/.config/zed` (fresh setup):
     ```bash
     git clone <repo-url> ~/.config/zed
     ```
   - Or copy/sync from another location:
     ```bash
     rsync -av --exclude .git /path/to/this/repo/ ~/.config/zed/
     ```
4. Launch Zed. Changes in `settings.json` and `keymap.json` load automatically.

## Quick Verification
- Settings: Zed → Command Palette → `Open Settings` → confirm your preferences.
- Keybindings: Zed → Command Palette → `Open Key Bindings` → check custom bindings.
- Themes: Zed → Command Palette → `Select Color Theme` → find themes from `themes/`.

## Notes
- Keep this folder as a git repo to version your editor config.
- Consider excluding `conversations/` if you don't want AI history in git.
- After updates to this repo, run `git pull` in `~/.config/zed` and restart Zed if needed.

## Official Docs
- [Getting Started](https://zed.dev/docs/)
- [Configuring Zed](https://zed.dev/docs/configuring-zed)
- [Key bindings](https://zed.dev/docs/key-bindings)
- [Themes](https://zed.dev/docs/themes)
- [Snippets](https://zed.dev/docs/snippets)
