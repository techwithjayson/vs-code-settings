
# VS Code — Settings & Extensions Setup

**Purpose**: Quick steps to apply the workspace VS Code settings and install the recommended extensions.

**Quick Setup**
- **Open Settings (JSON):** Press `Ctrl+Shift+P` and run _Preferences: Open Settings (JSON)_.
- **Apply settings:** Replace or merge your settings with the contents of [settings.json](settings.json).

**Recommended Extensions**
- **Prettier - Code formatter**: ensures consistent formatting (configured as the default formatter).
- **ESLint**: linting and fix-on-save support (`source.fixAll.eslint` used in settings).
- **GitLens — Git supercharged**: enhanced git awareness and the AI settings referenced in the config.
- **vscode-icons**: file icons (matches `workbench.iconTheme`).
- **Live Server**: for quick HTML/EJS live preview (the settings reference live server behavior).
- **GitHub Copilot**: AI coding assistant (settings enable Copilot in several languages).
- **Claude / ClaudeCode** (optional): if you use Anthropic/Claude integrations — settings reference `claudeCode`.

Additional recommended extensions
- **Night Owl (theme)**: match the workspace color theme.
- **MDX (MDX support)**: MDX syntax highlighting and editing support.
- **Tailwind CSS IntelliSense**: utility classes completion and linting for Tailwind projects.
- **Image Preview / Previewer**: enhanced image previews in the editor and markdown.
- **GitHub Actions (CI)**: workflows editing and validation helpers.
- **Dev Containers**: develop inside containers using `.devcontainer` setups.
- **Remote - Containers / Container Tools**: container management and tooling integration.
- **MobileView (HTML/CSS live preview)**: for mobile preview of HTML/CSS changes.
- **Code Spell Checker**: basic spell checking in code and markdown.
- **Powershell Extension Pack**: if you work with PowerShell, this pack includes the main extensions for that.
- **Prettier ESLint**: if you want a combined extension that runs Prettier and ESLint together.

Install extensions via the Extensions view (`Ctrl+Shift+X`) by searching each name and clicking **Install**.

**After Installing**
- Reload VS Code: `Ctrl+Shift+P` → _Developer: Reload Window_.
- Verify formatting and linting: open a JavaScript/HTML file and save to confirm `prettier` & `eslint` behavior.

**Notes & Tips**
- `prettier.requireConfig` is set to `true` in the workspace settings — Prettier will only run if a project has a Prettier configuration.
- The full workspace settings used here are in [settings.json](settings.json). Copy them into your user or workspace settings as desired.

If you want, I can:
- add `code --install-extension` commands for each extension, or
- create a small setup script to automate installing these extensions.

Quick copyable install commands (optional)
Run these in a terminal to install the most common extensions by name — verify marketplace IDs for your preferred variants if you prefer different publishers.

```bash
# Themes & UI
code --install-extension sdras.night-owl
code --install-extension vscode-icons-team.vscode-icons

# Formatting & linting
code --install-extension esbenp.prettier-vscode
code --install-extension dbaeumer.vscode-eslint

# Tailwind & MDX
code --install-extension bradlc.vscode-tailwindcss
code --install-extension silvenon.vscode-mdx

# Git & CI
code --install-extension eamodio.gitlens
code --install-extension GitHub.vscode-pull-request-github
code --install-extension GitHub.vscode-github-actions

# Containers & tooling
code --install-extension ms-vscode-remote.remote-containers
code --install-extension ms-vscode-remote.vscode-dev-containers
code --install-extension ms-azuretools.vscode-docker

# AI / Copilot (optional)
code --install-extension GitHub.copilot
```
