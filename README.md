# 💻 VS Code Setup for Frontend Developers

> My personal Visual Studio Code configuration for frontend development using React, Next.js, TypeScript, Tailwind CSS, and GitHub Copilot.

---

## ✨ Extensions

| Extension                 | Description                            |
| ------------------------- | -------------------------------------- |
| Auto Close Tag            | Automatically adds closing tags        |
| Auto Rename Tag           | Renames paired HTML/XML tags           |
| Better Comments           | Organize comments with colors          |
| Code Spell Checker        | Finds typos in code                    |
| DotENV                    | Syntax highlighting for `.env` files   |
| Error Lens                | Shows inline errors and warnings       |
| ES7+ React/Redux Snippets | Shorthand snippets for React and Redux |
| ESLint                    | Integrates ESLint with VS Code         |
| GitHub Copilot            | AI pair programmer                     |
| GitHub Copilot Chat       | Chat-based AI code support             |
| gitignore                 | Syntax support for `.gitignore`        |
| GitLens                   | Powerful Git insights                  |
| Import Cost               | Shows size of imported npm packages    |
| JavaScript (ES6) Snippets | Common JavaScript snippets             |
| Live Server (Five Server) | Local dev server with live reload      |
| Markdown Preview Enhanced | Rich markdown preview                  |
| npm Intellisense          | Autocompletes npm module imports       |
| Path Intellisense         | Autocompletes relative file paths      |
| Prettier - Code Formatter | Format your code consistently          |
| Tailwind CSS IntelliSense | IntelliSense for Tailwind classes      |
| Thunder Client            | Lightweight REST client                |
| VS Code Icons             | File icons for your workspace          |

---

## ⚙️ Settings

Here's the content of my `settings.json` for VS Code:

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

  // File Management
  "files.autoSave": "onFocusChange",
  "javascript.updateImportsOnFileMove.enabled": "always",
  "typescript.updateImportsOnFileMove.enabled": "always",

  // Terminal Settings
  "terminal.integrated.fontSize": 13,
  "terminal.integrated.defaultLocation": "editor",
  "terminal.integrated.fontFamily": "'Fira Code', Consolas, 'Courier New', monospace",
  "terminal.integrated.shellIntegration.enabled": true,
  "terminal.integrated.shellIntegration.decorationsEnabled": "gutter",

  // Git Settings
  "git.enableSmartCommit": true,
  "git.autofetch": true,

  // GitHub Copilot
  "github.copilot.enable": {
    "*": true
  },
  "github.copilot.nextEditSuggestions.enabled": true,

  // Folder Excludes
  "files.exclude": {
    "node_modules": true,
    "dist": true,
    ".next": true,
    "build": true
  },
  "search.exclude": {
    "node_modules": true,
    "dist": true,
    ".next": true,
    "build": true
  },

  // Tailwind Class Regex for IntelliSense
  "tailwindCSS.experimental.classRegex": [
    ["clsx\\(([^)]*)\\)", "(?:'|\"|`)([^']*)(?:'|\"|`)"],
    ["cn\\(([^)]*)\\)", "(?:'|\"|`)([^']*)(?:'|\"|`)"]
  ]
}
```
