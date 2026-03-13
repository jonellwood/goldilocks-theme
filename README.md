# 🐻 Goldilocks Theme for VS Code

> *Not too light. Not too dark. Just right.*

A medium-contrast VS Code theme for developers who don't live in extremes. Goldilocks sits comfortably between the eye-strain of blindingly white light themes and the endless void of pure black dark themes — landing somewhere around the perceptual midpoint where everything is actually readable without squinting or dilating.

---

## Color Philosophy

The base background is **#2e3440** — a dark slate blue-grey that's roughly 25% luminance. Dark themes are typically 5–12%, light themes are 85%+. Goldilocks lives in the comfortable middle.

| Role              | Color     | Why |
|------------------|-----------|-----|
| Background        | `#2e3440` | Neutral slate — not void-black, not eye-watering |
| Foreground text   | `#d0d8e8` | Soft blue-white — readable without burning |
| Keywords          | `#9080c0` | Medium purple — distinct, not harsh |
| Strings           | `#8ab870` | Muted green — classic, not neon |
| Functions         | `#70b8d0` | Cool teal — clean and calm |
| Numbers           | `#c09868` | Warm amber — naturally distinct |
| Classes/Types     | `#d8c068` | Golden yellow — stands out just right |
| Comments          | `#5a7070` | Dim teal — present but not intrusive |
| Accent (cursor)   | `#f0a84a` | Orange — energetic focal point |

---

## Language Support

Specifically tuned for:

- **PHP** — `$variables`, `->arrows`, `::colons`, namespaces, tags
- **JavaScript / TypeScript** — control flow, decorators, imports, template literals
- **HTML** — tags, attributes, entities, doctype
- **CSS** — selectors, properties, values, at-rules, `!important`
- **Vue.js** — component tags, `v-` directives, `{{ mustache }}` delimiters
- **SQL (SQL Server)** — keywords, functions, table/column names
- **JSON** — keys vs values distinctly colored
- **Markdown** — headings, bold, italic, links, code

---

## Installation

### From Source (during development)

1. Clone or copy this folder to your VS Code extensions directory:
   - **macOS/Linux:** `~/.vscode/extensions/goldilocks-theme`
   - **Windows:** `%USERPROFILE%\.vscode\extensions\goldilocks-theme`
2. Restart VS Code
3. Open Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
4. Run **Preferences: Color Theme**
5. Select **Goldilocks – Just Right**

### From VSIX (packaged)

```bash
# Install the vsce tool
npm install -g @vscode/vsce

# Package the theme from the theme folder
vsce package

# Install the resulting .vsix file
code --install-extension goldilocks-theme-1.0.0.vsix
```

---

## Publishing to the VS Code Marketplace

1. Create a free account at https://marketplace.visualstudio.com
2. Generate a Personal Access Token (PAT) in Azure DevOps
3. Update `publisher` in `package.json` to your publisher name
4. Run:
   ```bash
   npm install -g @vscode/vsce
   vsce login your-publisher-name
   vsce publish
   ```

---

## Tweaking the Theme

All colors are in `themes/goldilocks-color-theme.json`.

- **`colors`** — controls the VS Code UI (sidebar, tabs, terminal, status bar, etc.)
- **`tokenColors`** — controls syntax highlighting (what the grammar scopes target)
- **`semanticTokenColors`** — TypeScript/JS smarter highlighting layer

The comments in the file group everything logically so it's easy to find what to change.

---

*Made with 🥣 — because Goldilocks was right about everything.*
