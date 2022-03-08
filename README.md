# vscode-settings

A personal style guide for code in Visual Studio Code. 🚧



## Links

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

**Option 1**

- [Operator Mono](https://coding-fonts.css-tricks.com/fonts/operator-mono/)
  - Designed by Andy Clymer and Hoefler & Co

**Option 2**

- [Fira Code Retina](https://github.com/tonsky/FiraCode)
  - Free monospaced font with programming ligatures.

### Theme/Color

**Option 1**

- [One Dark Pro](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme)
  
  - Atom‘s iconic One Dark theme for Visual Studio Code

- [Nomo Dark Icon Theme](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-icontheme-nomo-dark)
  
  - Nomo Dark Icon Theme

**Option 2**

- [Dracula](https://marketplace.visualstudio.com/items?itemName=dracula-theme.theme-dracula)
  - Official Dracula Theme. A dark theme for many editors, shells, and more.
- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
  - Material Design Icons for Visual Studio Code.

### Workflow

- [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
  - Automatically add HTML/XML close tag.
- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
  - Automatically rename paired HTML/XML tag.
- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
  - Improve your code commenting by annotating with alert, informational, TODOs, and more!
- Fig
  - Companion extension for Fig to help integrate with VS Code
- [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
  - View a Git Graph of your repository, and perform Git actions from the graph.
- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
  - For git version history
- [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
  - Display import/require package size in the editor
- [LottieFiles for VS Code](https://marketplace.visualstudio.com/items?itemName=lottiefiles.vscode-lottie)
  - View and edit Lottie and dotLottie files.
- Todo Tree
  - Show TODO, FIXME, etc. comment tags in a tree view

### IntelliSense/AutoComplete

- [IntelliSense for css class names in html](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
  - CSS class name completion for the HTML class attribute based on the definitions found in your workspace.
- [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
  - Autocompletes npm modules in import/require statements
- [Path intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
  - Autocompletes filenames.
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
  - All you need to write Markdown (keyboard shortcuts, table of contents, auto preview and more).
- [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
  - Intelligent Tailwind CSS tooling for VS Code
- [Rocketseat ReactJS](https://marketplace.visualstudio.com/items?itemName=rocketseat.RocketseatReactJS)
  - ReactJS snippets created by Rocketseat.
- [HTML Snippets](https://marketplace.visualstudio.com/items?itemName=abusaidm.html-snippets)
  - Full HTML tags including HTML5 Snippets.
- [Jest Snippets](https://marketplace.visualstudio.com/items?itemName=andys8.jest-snippets)
  - Code snippets for testing framework Jest

### Style/Formatting

- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  - Integrates ESLint JS.
- [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
  - EditorConfig Support for Visual Studio Code.
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
  - Code formatter using prettier.
- [VS Code Styled Components](https://marketplace.visualstudio.com/items?itemName=jpoissonnier.vscode-styled-components)
  - Syntax highlighting for styled-components.
- [Color Highlight](https://marketplace.visualstudio.com/items?itemName=naumovs.color-highlight)
  - Highlight web colors in your editor.
- [DotENV](https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv)
  - Support for dotenv file syntax.
- [ES7+ React/Redux/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
  - Extensions for React, React-Native and Redux in JS/TS with ES7+ syntax. Customizable. Built-in integration with prettier.
- [Prisma](https://marketplace.visualstudio.com/items?itemName=Prisma.prisma)
  - Adds syntax highlighting, formatting, auto-completion, jump-to-definition and linting for .prisma files.
- [TypeScript Hero](https://marketplace.visualstudio.com/items?itemName=rbbit.typescript-hero)
  - Additional toolings for typescript

## settings.json

```json
{
  "editor.fontSize": 20,
  "editor.lineHeight": 30,
  "editor.letterSpacing": 0.4,
  "editor.cursorStyle": "line",
  "editor.hover.delay": 1500,
  "editor.quickSuggestions": {
    "other": true,
    "comments": false,
    "strings": false
  },
  "editor.showDeprecated": true,
  "editor.fontFamily": "Operator Mono SSm Lig",
  "editor.fontLigatures": true,
  "outline.icons": true,
  "editor.rulers": [80, 120],
  "editor.formatOnSave": true,
  "editor.linkedEditing": true,
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.renderLineHighlight": "gutter",
  "editor.tabSize": 2,
  "editor.parameterHints.enabled": false,
  "editor.minimap.enabled": false,
  "eslint.packageManager": "yarn",
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    }
  },
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    }
  },
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    }
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.codeActionsOnSave": {
      "source.fixAll": true
    }
  },
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.codeActionsOnSave": {
      "source.fixAll": true
    }
  },
  "[sql]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.codeActionsOnSave": {
      "source.fixAll": true
    }
  },
  "[markdown]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "editor.codeActionsOnSave": {
      "source.fixAll": true
    }
  },
  "[prisma]": {
    "editor.defaultFormatter": "Prisma.prisma"
  },
  "explorer.compactFolders": false,
  "files.associations": {
    ".sequelizerc": "javascript",
    ".stylelintrc": "json",
    ".prettierrc": "json"
  },
  "terminal.integrated.fontSize": 20,
  "terminal.integrated.fontFamily": "Operator Mono",
  "extensions.ignoreRecommendations": true,
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  },
  "emmet.includeLanguages": {
    "javascript": "javascriptreact"
  },
  "breadcrumbs.enabled": true,
  "git.enableSmartCommit": true,
  "javascript.updateImportsOnFileMove.enabled": "never",
  "typescript.updateImportsOnFileMove.enabled": "never",
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "typescript.tsserver.log": "off",
  "javascript.suggest.autoImports": true,
  "auto-close-tag.enableAutoCloseTag": true,
  "auto-close-tag.activationOnLanguage": [
    "xml",
    "javascriptreact",
    "typescriptreact",
    "markdown",
    "vue",
    "HTML (Eex)"
  ],
  "auto-rename-tag.activationOnLanguage": [
    "xml",
    "javascriptreact",
    "typescriptreact",
    "markdown",
    "vue",
    "HTML (Eex)"
  ],
  "npm-intellisense.importES6": true,
  "npm-intellisense.importQuotes": "'",
  "npm-intellisense.importLinebreak": ";\r\n",
  "npm-intellisense.importDeclarationType": "const",
  "npm-intellisense.scanDevDependencies": true,
  "importCost.smallPackageColor": "#44475a",
  "importCost.mediumPackageColor": "#44475a",
  "importCost.largePackageColor": "#44475a",
  "workbench.startupEditor": "newUntitledFile",
  "workbench.activityBar.visible": true,
  "workbench.iconTheme": "vs-nomo-dark",
  "workbench.colorTheme": "One Dark Pro Flat",
  "workbench.colorCustomizations": {
    "badge.background": "#61afef",
    "activityBarBadge.background": "#61afef"
  },
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": ["comment", "punctuation.definition.comment"],
        "settings": {
          "foreground": "#404754"
        }
      },
      {
        "scope": ["variable.other.readwrite"],
        "settings": {
          "foreground": "#e5c07b"
        }
      }
    ]
  },
  "todo-tree.general.tags": ["_bug", "_fix", "_note"],
  "todo-tree.general.statusBar": "tags",
  "todo-tree.tree.tagsOnly": false,
  "todo-tree.highlights.defaultHighlight": {
    "type": "line",
    "fontWeight": "bold",
    "foreground": "#f0f0f0",
    "background": "#404754",
    "gutterIcon": true
  },
  "todo-tree.highlights.customHighlight": {
    "_note": {
      "foreground": "#e5c07b",
      "iconColour": "#e5c07b",
      "icon": "info"
    },
    "_fix": {
      "foreground": "#c678dd",
      "iconColour": "#c678dd",
      "icon": "tools"
    },
    "_bug": {
      "foreground": "#e06c75",
      "iconColour": "#e06c75",
      "icon": "zap"
    }
  },
  "terminal.integrated.env.osx": {
    "FIG_NEW_SESSION": "1"
  },
  "editor.accessibilitySupport": "off",
  "reactSnippets.settings.typescript": true,
  "reactSnippets.settings.prettierEnabled": true,
  "reactSnippets.settings.importReactOnTop": true,
  "reactSnippets.settings.typescriptPropsStatePrefix": "type",
  "reactSnippets.settings.languageScopes": "typescript,typescriptreact,javascript,javascriptreact"
}
```

## keybindings.json

> Note: Some keys bindings maybe not be available on windows system. See more about key bindings for windows in [offcial site](https://code.visualstudio.com/docs/getstarted/keybindings).

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
