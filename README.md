<div align="center">

# 🌿 VS Code Config

**A dark-green, front-end focused Visual Studio Code setup built for React, Tailwind CSS and Sass.**

![VS Code](https://img.shields.io/badge/VS%20Code-Settings-007ACC?logo=visualstudiocode&logoColor=white)
![Extensions](https://img.shields.io/badge/Extensions-20-63a67b)
![Theme](https://img.shields.io/badge/Theme-Andromeda%20%2B%20Forest%20Green-08140b)
![Formatter](https://img.shields.io/badge/Formatter-Prettier-F7B93E?logo=prettier&logoColor=black)
![Linting](https://img.shields.io/badge/Lint-ESLint%20%2B%20Stylelint-4B32C3?logo=eslint&logoColor=white)

</div>

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Highlights](#-highlights)
- [Color Palette](#-color-palette)
- [Extensions](#-extensions)
- [Installation](#-installation)
- [Full settings.json (Copy & Paste)](#-full-settingsjson-copy--paste)
- [Settings Breakdown](#-settings-breakdown)
- [Customization](#-customization)
- [Contributing](#-contributing)
- [Author](#-author)

---

## 🔎 Overview

This repository contains my personal `settings.json` and the full list of extensions I use for daily web development. The setup is tuned for:

- ⚛️ **React** and modern JavaScript / TypeScript
- 🎨 **Tailwind CSS** and **Sass/SCSS** workflows
- 🧹 Automatic **formatting and linting on save**
- 👀 A low-glare **forest-green dark theme** layered on top of *Andromeda*

---

## ✨ Highlights

| Area | What you get |
| --- | --- |
| **Editor** | 20px font, 32px line height, word wrap, smooth scrolling and an expanding cursor animation |
| **Formatting** | Prettier on save and paste, with ESLint and Stylelint auto-fix on save |
| **Productivity** | Linked editing, bracket pair colorization and guides, Emmet in JSX, Tailwind class completion inside strings |
| **Tooltips** | Hovers only appear while holding `Alt`, so they stay out of the way |
| **Auto save** | Files save automatically when the editor loses focus |
| **Terminal** | Git Bash on Windows, Bash on Linux, matching theme and 20px font |
| **Live preview** | Live Server opens Chrome in private mode, and Live Sass Compiler outputs minified CSS |
| **Presenting** | Screencast Mode is configured to show only keyboard shortcuts |

---

## 🎨 Color Palette

The workbench uses a custom green palette defined in `workbench.colorCustomizations` and `editor.tokenColorCustomizations`.

| Role | Hex | Used for |
| --- | --- | --- |
| Editor background | `#08140b` | Editor, sidebar, minimap, terminal |
| Deep background | `#050d07` | Activity bar, inactive tabs, tab strip |
| Active tab | `#122919` | Active tab, scrollbar, terminal border |
| Status bar | `#0d1f13` | Status bar background |
| Foreground | `#c2ddc7` | Default text and variables |
| Muted text | `#8ba892` | Activity bar and status bar icons |
| Comments | `#567a61` | Comments (italic) |
| Strings | `#93c7a3` | String literals |
| Keywords | `#63a67b` | Keywords, storage, language variables |
| Functions | `#78b88d` | Function names |
| Constants | `#b1d1b7` | Numbers and constants |
| Line numbers | `#33543d` | Gutter line numbers |

---

## 🧩 Extensions

**20 extensions** in total, grouped by purpose.

### 🎨 Theme & Appearance

| Extension | Publisher | Marketplace ID |
| --- | --- | --- |
| Andromeda | Eliver Lara | `EliverLara.andromeda` |
| Material Icon Theme | Philipp Kief | `PKief.material-icon-theme` |
| indent-rainbow | oderwat | `oderwat.indent-rainbow` |
| Error Lens | Alexander | `usernamehw.errorlens` |

### 🛠️ Formatting & Linting

| Extension | Publisher | Marketplace ID |
| --- | --- | --- |
| Prettier - Code formatter | Prettier | `esbenp.prettier-vscode` |
| ESLint | Microsoft | `dbaeumer.vscode-eslint` |
| Stylelint | Stylelint | `stylelint.vscode-stylelint` |

### ⚡ Productivity & IntelliSense

| Extension | Publisher | Marketplace ID |
| --- | --- | --- |
| Auto Close Tag | Jun Han | `formulahendry.auto-close-tag` |
| Auto Rename Tag | Jun Han | `formulahendry.auto-rename-tag` |
| Auto Import - ES6, TS, JSX, TSX | Sergey Korenuk | `NuclleaR.vscode-extension-auto-import` |
| Path Intellisense | Christian Kohler | `christian-kohler.path-intellisense` |
| npm Intellisense | Christian Kohler | `christian-kohler.npm-intellisense` |
| HTML CSS Support | ecmel | `ecmel.vscode-html-css` |
| Tailwind CSS IntelliSense | Tailwind Labs | `bradlc.vscode-tailwindcss` |

### 📝 Snippets

| Extension | Publisher | Marketplace ID |
| --- | --- | --- |
| JavaScript (ES6) code snippets | charalampos karypidis | `xabikos.JavaScriptSnippets` |
| Reactjs code snippets | charalampos karypidis | `xabikos.ReactSnippets` |
| Simple React Snippets | Burke Holland | `burkeholland.simple-react-snippets` |

### 🚀 Tooling

| Extension | Publisher | Marketplace ID |
| --- | --- | --- |
| Live Server | Ritwick Dey | `ritwickdey.LiveServer` |
| Live Sass Compiler | Glenn Marks | `glenn2223.live-sass` |
| Snipped | Jefferson Licet | `jeffersonlicet.snipped` |

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/AbdullahProBD/VS-Code-Config.git
cd VS-Code-Config
```

### 2. Install all extensions at once

**macOS / Linux / Git Bash**

```bash
for ext in \
  EliverLara.andromeda \
  PKief.material-icon-theme \
  oderwat.indent-rainbow \
  usernamehw.errorlens \
  esbenp.prettier-vscode \
  dbaeumer.vscode-eslint \
  stylelint.vscode-stylelint \
  formulahendry.auto-close-tag \
  formulahendry.auto-rename-tag \
  NuclleaR.vscode-extension-auto-import \
  christian-kohler.path-intellisense \
  christian-kohler.npm-intellisense \
  ecmel.vscode-html-css \
  bradlc.vscode-tailwindcss \
  xabikos.JavaScriptSnippets \
  xabikos.ReactSnippets \
  burkeholland.simple-react-snippets \
  ritwickdey.LiveServer \
  glenn2223.live-sass \
  jeffersonlicet.snipped
do
  code --install-extension "$ext"
done
```

**Windows (PowerShell)**

```powershell
@(
  "EliverLara.andromeda", "PKief.material-icon-theme", "oderwat.indent-rainbow",
  "usernamehw.errorlens", "esbenp.prettier-vscode", "dbaeumer.vscode-eslint",
  "stylelint.vscode-stylelint", "formulahendry.auto-close-tag",
  "formulahendry.auto-rename-tag", "NuclleaR.vscode-extension-auto-import",
  "christian-kohler.path-intellisense", "christian-kohler.npm-intellisense",
  "ecmel.vscode-html-css", "bradlc.vscode-tailwindcss", "xabikos.JavaScriptSnippets",
  "xabikos.ReactSnippets", "burkeholland.simple-react-snippets",
  "ritwickdey.LiveServer", "glenn2223.live-sass", "jeffersonlicet.snipped"
) | ForEach-Object { code --install-extension $_ }
```

### 3. Apply the settings

Copy `settings.json` into your VS Code user folder, or paste its contents via
**Command Palette → `Preferences: Open User Settings (JSON)`**.
Prefer a quick copy? Jump to the [full config below](#-full-settingsjson-copy--paste) and use the copy button.

| OS | User settings path |
| --- | --- |
| Windows | `%APPDATA%\Code\User\settings.json` |
| macOS | `~/Library/Application Support/Code/User/settings.json` |
| Linux | `~/.config/Code/User/settings.json` |

> 💡 **Tip:** Back up your current `settings.json` before overwriting it.

### 4. Reload

Run **`Developer: Reload Window`** from the Command Palette and the theme will be applied.

---

## 📋 Full settings.json (Copy & Paste)

Click the **copy** button at the top-right of the code block, then paste it into
**Command Palette → `Preferences: Open User Settings (JSON)`**, replacing the existing contents.

> ⚠️ Install the [extensions](#-extensions) first, otherwise VS Code will flag the extension-specific keys as unknown.

```jsonc
{
  // ───────────── Editor ─────────────
  "editor.fontSize": 20,
  "editor.lineHeight": 32,
  "editor.tabSize": 2,
  "editor.wordWrap": "on",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorBlinking": "expand",
  "editor.smoothScrolling": true,
  "editor.linkedEditing": true,
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": true,
  "editor.guides.bracketPairsHorizontal": true,
  "editor.hover.enabled": "onKeyboardModifier", // hold Alt to see hovers
  "editor.quickSuggestions": {
    "other": "on",
    "comments": "off",
    "strings": "on", // needed for Tailwind class completion
  },
  "editor.colorDecorators": true, // color swatches before hex/rgba values
  "editor.defaultColorDecorators": "always",
  "window.zoomLevel": 1,

  // ───────────── Formatting / Save ─────────────
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features",
  },
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit",
    "source.fixAll.stylelint": "explicit",
  },
  "files.autoSave": "onFocusChange",

  // ───────────── Theme / Colors ─────────────
  "workbench.colorTheme": "Andromeda",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.editor.enablePreview": false,
  "workbench.startupEditor": "none",
  "workbench.colorCustomizations": {
    "editor.background": "#08140b",
    "editor.foreground": "#c2ddc7",
    "editorGroupHeader.tabsBackground": "#050d07",
    "activityBar.background": "#050d07",
    "activityBar.foreground": "#8ba892",
    "sideBar.background": "#08140b",
    "minimap.background": "#08140b",
    "tab.activeBackground": "#122919",
    "tab.activeForeground": "#c2ddc7",
    "tab.inactiveBackground": "#050d07",
    "terminal.border": "#122919",
    "terminal.background": "#08140b",
    "statusBar.background": "#0d1f13",
    "statusBar.foreground": "#8ba892",
    "scrollbarSlider.background": "#122919",
    "scrollbarSlider.hoverBackground": "#1e3d27",
    "editorLineNumber.foreground": "#33543d",
  },
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": ["comment", "punctuation.definition.comment"],
        "settings": { "foreground": "#567a61", "fontStyle": "italic" },
      },
      {
        "scope": ["string"],
        "settings": { "foreground": "#93c7a3" },
      },
      {
        "scope": ["keyword", "storage", "variable.language"],
        "settings": { "foreground": "#63a67b" },
      },
      {
        "scope": ["variable", "entity.name.variable", "support.variable"],
        "settings": { "foreground": "#c2ddc7" },
      },
      {
        "scope": ["entity.name.function", "support.function"],
        "settings": { "foreground": "#78b88d" },
      },
      {
        "scope": [
          "constant.numeric",
          "constant.language",
          "constant.character",
        ],
        "settings": { "foreground": "#b1d1b7" },
      },
    ],
  },

  // ───────────── Terminal ─────────────
  "terminal.integrated.fontSize": 20,
  "terminal.integrated.defaultProfile.windows": "Git Bash",
  "terminal.integrated.defaultProfile.linux": "bash",
  "terminal.integrated.commandsToSkipShell": [
    "kilo-code.new.agentManagerOpen",
    "kilo-code.new.agentManager.showTerminal",
    "kilo-code.new.agentManager.previousTerminal",
    "kilo-code.new.agentManager.nextTerminal",
  ],

  // ───────────── Diff / Security / Git ─────────────
  "diffEditor.wordWrap": "on",
  "security.workspace.trust.untrustedFiles": "open",
  "git.enableSmartCommit": true,

  // ───────────── Prettier ─────────────
  "prettier.proseWrap": "preserve",
  "prettier.singleQuote": true,
  "prettier.arrowParens": "avoid",

  // ───────────── Emmet ─────────────
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
  },
  "emmet.triggerExpansionOnTab": true,

  // ───────────── Path Intellisense ─────────────
  // Disable built-in path suggestions to avoid duplicates
  "typescript.suggest.paths": false,
  "javascript.suggest.paths": false,
  "path-intellisense.mappings": {
    "@": "${workspaceFolder}/src",
  },
  "path-intellisense.autoSlashAfterDirectory": true,

  // ───────────── npm Intellisense ─────────────
  "npm-intellisense.importES6": true,
  "npm-intellisense.importQuotes": "'",
  "npm-intellisense.scanDevDependencies": true,
  "npm-intellisense.recursivePackageLookup": true,

  // ───────────── Stylelint (disable built-in CSS linting) ─────────────
  "css.validate": false,
  "scss.validate": false,
  "less.validate": false,
  "css.lint.unknownAtRules": "ignore", // allows @tailwind / @apply

  // ───────────── Tailwind CSS IntelliSense ─────────────
  "tailwindCSS.emmetCompletions": true,
  "tailwindCSS.colorDecorators": true,
  "tailwindCSS.experimental.classRegex": [
    ["clsx\\(([^)]*)\\)", "(?:'|\"|`)([^']*)(?:'|\"|`)"],
    ["cva\\(([^)]*)\\)", "[\"'`]([^\"'`]*).*?[\"'`]"],
  ],

  // ───────────── Error Lens ─────────────
  "errorLens.enabledDiagnosticLevels": ["error", "warning"],
  "errorLens.delay": 300,

  // ───────────── Live Server ─────────────
  "liveServer.settings.CustomBrowser": "chrome:PrivateMode",
  "liveServer.settings.donotShowInfoMsg": true,
  "liveServer.settings.donotVerifyTags": true,
  "liveServer.settings.ignoreFiles": [".vscode/**", "**/*.scss", "**/*.sass"],

  // ───────────── Live Sass Compiler ─────────────
  "liveSassCompile.settings.formats": [
    {
      "format": "compressed",
      "extensionName": ".min.css",
      "savePath": "/css",
    },
  ],
  "liveSassCompile.settings.generateMap": false,
  "liveSassCompile.settings.excludeList": ["**/node_modules/**", ".vscode/**"],
  "liveSassCompile.settings.autoprefix": ["> 1%", "last 2 versions"],

  // ───────────── Screencast Mode ─────────────
  "screencastMode.onlyKeyboardShortcuts": true,
  "screencastMode.mouseIndicatorColor": "#63a67b",
  "screencastMode.verticalOffset": 0,

  // ───────────── AI / Misc ─────────────
  "chat.editing.confirmEditRequestRetry": false,
  "kilo-code.new.showTaskTimeline": false,
  "github.copilot.enable": {
    "*": false,
    "plaintext": false,
    "markdown": false,
    "scminput": false,
    "json": false,
  },
  "git.confirmSync": false,
}
```

---

## ⚙️ Settings Breakdown

<details>
<summary><b>Editor</b></summary>

- `editor.fontSize: 20` and `editor.lineHeight: 32` for comfortable reading
- `editor.wordWrap: on` so long lines never scroll sideways
- `editor.cursorBlinking: expand` and `cursorSmoothCaretAnimation` for smooth cursor movement
- `editor.hover.enabled: onKeyboardModifier` shows hovers only while `Alt` is held
- `editor.quickSuggestions.strings: on`, which is required for Tailwind class completion
- `editor.linkedEditing: true` renames paired HTML tags together

</details>

<details>
<summary><b>Formatting & Save</b></summary>

- Prettier is the default formatter, running on save and paste
- HTML files use VS Code's built-in HTML formatter instead of Prettier
- ESLint and Stylelint `fixAll` run explicitly on save
- `files.autoSave: onFocusChange`
- Prettier options: single quotes, `arrowParens: avoid`, `proseWrap: preserve`

</details>

<details>
<summary><b>CSS / Tailwind</b></summary>

- Built-in CSS, SCSS and Less validation is disabled so Stylelint is the single source of truth
- `css.lint.unknownAtRules: ignore` allows `@tailwind` and `@apply`
- `tailwindCSS.experimental.classRegex` adds class detection inside `clsx()` and `cva()`
- Tailwind Emmet completions and color decorators are enabled

</details>

<details>
<summary><b>Path & npm IntelliSense</b></summary>

- Built-in TS/JS path suggestions are disabled to avoid duplicates
- Alias `@` maps to `${workspaceFolder}/src`
- npm Intellisense imports with ES6 syntax and single quotes, and scans `devDependencies`

</details>

<details>
<summary><b>Live Server & Sass</b></summary>

- Live Server opens Chrome in private mode and ignores `.vscode` and Sass files
- Live Sass Compiler outputs compressed `.min.css` into `/css`, with autoprefixer for `> 1%, last 2 versions`
- Source maps are disabled and `node_modules` is excluded

</details>

<details>
<summary><b>Terminal & Git</b></summary>

- Default terminal: Git Bash on Windows, Bash on Linux
- `git.enableSmartCommit: true` and `git.confirmSync: false` for a faster commit flow

</details>

---

## 🛠️ Customization

A few settings you may want to change for your own machine:

- **`window.zoomLevel` and font sizes (`20`)**: lower these on smaller screens.
- **`terminal.integrated.defaultProfile.windows`**: change if you do not use Git Bash.
- **`liveServer.settings.CustomBrowser`**: swap `chrome:PrivateMode` for your preferred browser.
- **`path-intellisense.mappings`**: update the `@` alias if your source folder is not `src`.
- **`kilo-code.*` and `chat.*` entries**: these only apply if you use the Kilo Code extension, so they can be removed otherwise.
- **`github.copilot.enable`**: Copilot is disabled for all languages in this config. Remove the block to re-enable it.
- **`workbench.colorCustomizations`**: edit the hex values to create your own color variant.

---

## 🤝 Contributing

Suggestions and improvements are welcome.

1. Fork the repository
2. Create a branch: `git checkout -b feature/my-improvement`
3. Commit your changes: `git commit -m "Add my improvement"`
4. Push the branch: `git push origin feature/my-improvement`
5. Open a Pull Request

---

## 👤 Author

**Abdullah**
GitHub: [@AbdullahProBD](https://github.com/AbdullahProBD)

---

<div align="center">

If this setup helped you, consider giving the repo a ⭐

</div>
