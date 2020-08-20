# vscode-settings

A personal style guide for code in VS Code. 🚧

## Liks

- [vscode-settings](#vscode-settings)
  - [Liks](#liks)
  - [Extensions](#extensions)
    - [Font](#font)
    - [Theme/Color](#themecolor)
    - [Workflow](#workflow)
    - [IntelliSense/AutoComplete](#intellisenseautocomplete)
    - [Style/Formatting](#styleformatting)
  - [settings.json](#settingsjson)
  - [keybindings.json](#keybindingsjson)

## Extensions

### Font

- [Fira Code Retina](https://github.com/tonsky/FiraCode)
  - Free monospaced font with programming ligatures.

### Theme/Color

- [Dracula](https://marketplace.visualstudio.com/items?itemName=dracula-theme.theme-dracula)
  - Official Dracula Theme. A dark theme for many editors, shells, and more.
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
  - Material Design Icons for Visual Studio Code.
- [Color Highlight](https://marketplace.visualstudio.com/items?itemName=naumovs.color-highlight)
  - Highlight web colors in your editor.
- [DotENV](https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv)
  - Support for dotenv file syntax.

### Workflow

- [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
  - Automatically add HTML/XML close tag.
- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
  - Automatically rename paired HTML/XML tag.
- [Rocketseat ReactJS](https://marketplace.visualstudio.com/items?itemName=rocketseat.RocketseatReactJS)
  - ReactJS snippets created by Rocketseat.
- [HTML Snippets](https://marketplace.visualstudio.com/items?itemName=abusaidm.html-snippets)
  - Full HTML tags including HTML5 Snippets.

### IntelliSense/AutoComplete

- [IntelliSense for css class names in html](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
  - CSS class name completion for the HTML class attribute based on the definitions found in your workspace.
- [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
  - Autocompletes npm modules in import/require statements
- [Path intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
  - Autocompletes filenames.
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
  - All you need to write Markdown (keyboard shortcuts, table of contents, auto preview and more).

### Style/Formatting

- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  - Integrates ESLint JS.
- [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
  - EditorConfig Support for Visual Studio Code.
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
  - Code formatter using prettier.
- [VS Code Styled Components](https://marketplace.visualstudio.com/items?itemName=jpoissonnier.vscode-styled-components)
  - Syntax highlighting for styled-components.

## settings.json

```json
{
  "editor.fontSize": 16,
  "editor.lineHeight": 24,
  "editor.fontFamily": "Fira Code Retina",
  "editor.fontLigatures": true,
  "editor.rulers": [80, 120],
  "editor.formatOnSave": true,
  "editor.renderLineHighlight": "gutter",
  "editor.tabSize": 2,
  //"eslint.packageManager": "yarn", // on osx
  "eslint.packageManager": "npm", // on linux
  "[javascript]": {
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    },
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascriptreact]": {
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    },
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    },
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescriptreact]": {
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    },
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[html]": {
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    },
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[css]": {
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    },
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "explorer.compactFolders": false,
  "files.associations": {
    ".sequelizerc": "javascript",
    ".stylelintrc": "json",
    ".prettierrc": "json"
  },
  "terminal.integrated.fontSize": 16,
  "terminal.integrated.fontFamily": "Fira Code Retina",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.startupEditor": "newUntitledFile",
  "window.zoomLevel": 0,
  "extensions.ignoreRecommendations": true,
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "javascript.updateImportsOnFileMove.enabled": "never",
  "breadcrumbs.enabled": true,
  "git.enableSmartCommit": true,
  "editor.parameterHints.enabled": false,
  "typescript.updateImportsOnFileMove.enabled": "never",
  "terminal.integrated.shell.osx": "/bin/zsh",
  "terminal.integrated.shell.linux": "usr/bin/zsh",
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "typescript.tsserver.log": "verbose",
  "javascript.suggest.autoImports": false,
  "typescript.suggest.autoImports": false,
  "workbench.activityBar.visible": true,
  "editor.minimap.enabled": false,
  "workbench.colorTheme": "Dracula",
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": [],
        "settings": {
          "fontStyle": "italic"
        }
      }
    ]
  },
  "emojisense.languages": {
    "markdown": true,
    "plaintext": false,
    "json": true,
    "html": true,
    "javascript": true,
    "scminput": true
  },
  "window.menuBarVisibility": "toggle",
  "auto-close-tag.enableAutoCloseTag": true,
  "auto-close-tag.activationOnLanguage": [
    "xml",
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "markdown",
    "vue",
    "HTML (Eex)"
  ],
  "auto-rename-tag.activationOnLanguage": [
    "xml",
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "markdown",
    "vue",
    "HTML (Eex)"
  ]
}
```

## keybindings.json

> Note: Some keys bindings maybe not be available on windows system. See more about key bindings for windows on [offcial site](https://code.visualstudio.com/docs/getstarted/keybindings).

```json
[
  {
    "key": "ctrl+'",
    "command": "workbench.action.terminal.focus"
  },
  {
    "key": "ctrl+.",
    "command": "emojisense.quickEmoji",
    "when": "editorTextFocus"
  },
  {
    "key": "ctrl+[Slash]",
    "command": "editor.action.commentLine",
    "when": "editorTextFocus"
  },
  {
    "key": "cmd+1",
    "command": "workbench.action.openEditorAtIndex1"
  },
  {
    "key": "alt+1",
    "command": "workbench.action.openEditorAtIndex1"
  },
  {
    "key": "cmd+2",
    "command": "workbench.action.openEditorAtIndex2"
  },
  {
    "key": "alt+2",
    "command": "workbench.action.openEditorAtIndex2"
  },
  {
    "key": "cmd+3",
    "command": "workbench.action.openEditorAtIndex2"
  },
  {
    "key": "alt+3",
    "command": "workbench.action.openEditorAtIndex2"
  },
  {
    "key": "cmd+4",
    "command": "workbench.action.openEditorAtIndex3"
  },
  {
    "key": "alt+4",
    "command": "workbench.action.openEditorAtIndex3"
  }
]
```
