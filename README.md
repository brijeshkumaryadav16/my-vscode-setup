# 💻 My VSCode Setup

This is my personal VS Code setup for frontend development. Feel free to use or adapt it for your own workflow!

---

## 1. Install VS Code

- Download from [code.visualstudio.com](https://code.visualstudio.com/)

---

## 2. Recommended Extensions

Search and install these extensions in VS Code. These help with code quality, productivity, and GitHub collaboration:

- Auto Close Tag
- Auto Rename Tag
- Better Comments
- Code Spell Checker
- DotENV
- Error Lens
- ES7+ React/Redux Snippets
- ESLint
- GitHub Copilot
- Github Copilot Chat
- gitignore
- GitLens
- Import Cost
- JavaScript (ES6) Snippets
- Live Server (Five Server)
- Markdown Preview Enhanced
- markdownlint
- MDX
- npm Intellisense
- Path Intellisense
- Prettier - Code Formatter
- Tailwind CSS IntelliSense
- vscode-icons

---

## 3. Install Fira Code Font

Fira Code improves code readability with ligatures.

- Download from [Fira Code GitHub Releases](https://github.com/tonsky/FiraCode/releases)
- Install the font on your system (double-click and "Install" on Mac/Windows)
- In VS Code, go to Settings → search "Font Family" → set to: `Fira Code, Consolas, 'Courier New', monospace`
- Enable font ligatures: search "Font Ligatures" in Settings and check the box

---

## 4. VS Code Settings

Copy and paste into your `settings.json` (open Command Palette → Preferences: Open Settings (JSON)):

```json
{
  // Editor Settings
  "editor.fontSize": 13,
  "editor.wordWrap": "on",
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnPaste": true,
  "editor.cursorBlinking": "expand",
  "editor.fontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "editor.fontLigatures": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "always",
    "source.organizeImports": "always"
  },
  "editor.formatOnSave": true,
  "editor.cursorStyle": "line",
  "editor.minimap.enabled": false,
  "workbench.iconTheme": "vscode-icons",
  "workbench.startupEditor": "none",
  "editor.accessibilitySupport": "off",

  // Workbench Settings
  "workbench.iconTheme": "vscode-icons",
  // The following setting ensures that files with the `.svg` extension open in the default code editor, allowing you to view and edit the SVG source code directly instead of seeing an icon preview.
  "workbench.editorAssociations": {
    "*.svg": "default"
  },

  // File Management
  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.updateImportsOnFileMove.enabled": "always",

  // Terminal Settings
  "terminal.integrated.fontSize": 13,
  "terminal.integrated.defaultLocation": "editor",
  "terminal.integrated.fontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "terminal.integrated.shellIntegration.enabled": true,
  "terminal.integrated.shellIntegration.decorationsEnabled": "gutter",
  "terminal.integrated.defaultProfile.osx": "zsh", // Window "PowerShell", Linux "bash" and Mac "zsh"
  "terminal.integrated.scrollback": 1000,
  "terminal.integrated.cursorBlinking": true,
  "terminal.integrated.cursorStyle": "line",
  "terminal.integrated.suggest.enabled": true,

  // Git Settings
  "git.enableSmartCommit": true,
  "git.autofetch": true,

  // GitHub Copilot
  "github.copilot.enable": {
    "*": true
  },
  "github.copilot.nextEditSuggestions.enabled": true,

  // Search & File Exclusions
  "search.exclude": {
    "node_modules": true,
    "dist": true,
    ".next": true,
    "build": true,
    ".git": true
  }
}
```

Thanks for checking out my VS Code setup.
