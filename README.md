# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production ap{
  "window.menuBarVisibility": "toggle",
  "window.commandCenter": false,
  "window.titleBarStyle": "native",
  
  "workbench.editor.labelFormat": "short",
  "workbench.activityBar.location": "hidden",
  "workbench.statusBar.visible": false,
  "workbench.layoutControl.enabled": false,
  "workbench.colorTheme": "Min Dark",
  "workbench.iconTheme": "symbols",
  "workbench.startupEditor": "newUntitledFile",
  
  "editor.tabSize": 2,
  "editor.fontSize": 14,
  "editor.lineHeight": 1.8,
  "editor.fontFamily": "JetBrains Mono",
  "editor.fontLigatures": true,
  "editor.rulers": [80, 120],
  "editor.semanticHighlighting.enabled": false,
  "editor.inlineSuggest.enabled": true,
  "editor.renderLineHighlight": "gutter",
  "editor.scrollbar.vertical": "hidden",
  "editor.scrollbar.horizontal": "hidden",
  "editor.parameterHints.enabled": false,
  "editor.guides.bracketPairs": true,

  "explorer.compactFolders" :  false,
  "explorer.fileNesting.enabled": true,
  "explorer.fileNesting.patterns": {
    "package.json": ".eslint*, prettier*, tsconfig*, vite*, yarn*, jest*, ormconfig*, babel*",
    "tailwind.config*": "tailwind.config*, postcss.config*",
    ".env": ".env*",
  },
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,

  "extensions.ignoreRecommendations": true,

  "breadcrumbs.enabled": false,

  "files.associations": {
    ".env.*": "dotenv",
    ".prettierrc": "json",
    "*.css": "css"
  },
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/node_modules": true
  },

  "emmet.includeLanguages": {"javascript": "javascriptreact"},
  "emmet.syntaxProfiles": {"javascript": "jsx"},

  "terminal.integrated.fontSize": 14,
  "terminal.integrated.fontFamily": "JetBrains Mono",
  "terminal.integrated.defaultProfile.windows": "Ubuntu-20.04 (WSL)",
  "terminal.integrated.env.linux": {},
  "terminal.integrated.profiles.windows": {
    "PowerShell": {
      "source": "PowerShell",
      "icon": "terminal-powershell"
    },
    "Command Prompt": {
      "path": [
        "${env:windir}\\Sysnative\\cmd.exe",
        "${env:windir}\\System32\\cmd.exe"
      ],
      "args": [],
      "icon": "terminal-cmd"
    },
    "Git Bash": {
      "source": "Git Bash"
    },
    "Ubuntu-20.04 (WSL)": {
      "path": "C:\\Windows\\System32\\wsl.exe",
      "args": [
        "-d",
        "Ubuntu-20.04"
      ]
    }
  },
 
  "security.workspace.trust.untrustedFiles": "open",
  
  "git.autofetch": true,
  "github.copilot.enable": {
    "*": true,
    "yaml": true,
    "plaintext": false,
    "markdown": true,
    "javascript": true,
    "python": true,
    "typescript": true
  },

  "javascript.updateImportsOnFileMove.enabled": "never", 
  "typescript.updateImportsOnFileMove.enabled": "never", 
  "javascript.suggest.autoImports": true,
  "typescript.suggest.autoImports": true,
  "typescript.preferences.renameMatchingJsxTags": false,
  "[javascript][javascriptreact][typescript][typescriptreact]": {
    "editor.codeActionsOnSave": {
      "source.fixAll.eslint": "explicit"
    }
  },
  "[python]": {
    "editor.formatOnType": true
  },
  "[json]": {
    "editor.defaultFormatter": "vscode.json-language-features"
  },
  "[prisma]": {
    "editor.formatOnSave": true
  },

  "symbols.hidesExplorerArrows": false,
  "symbols.files.associations": {
    "*.module.ts": "nest",
    "*.guard.ts": "typescript",
    "*.spec.ts": "ts-test",
    "*.e2e-spec.ts": "ts-test",
    "vitest.config.e2e.ts": "vite",
    ".env.example": "gear"
  },

  "liveServer.settings.CustomBrowser": "chrome",
  "liveServer.settings.donotShowInfoMsg": true,
}plication, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
# Ignite-Time
