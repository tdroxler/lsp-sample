# LSP Example

Copy/paste/adapted from https://github.com/microsoft/vscode-extension-samples/tree/main/lsp-sample

## Install

Change 

```
"activationEvents": [
    "onLanguage:scala"
]
```

In `package.json`

and 

```
let serverExe = '/nix/store/drz11xynmmcj4iwp94jb16qvfhd8mck5-system-path/bin/metals';
```

in `client/src/extension.ts`

then

```
npm i
npm run postinstall
npm run compile
npm run build
```

This create a `lsp-sample-1.0.0.vsix` file, you can install it from vscode (ctrl-shift-x) clique on the three dot `...` and select `Install from VSIX`.
