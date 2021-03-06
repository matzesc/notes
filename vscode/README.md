# Visual Studio Code

- Back to [Personal Notes](../README.md)

VS Code notes

- [Symbols & Outline Tree View](outline.md)

## Documentation

- [Getting Started](https://code.visualstudio.com/docs)
- [Get started with C# and Visual Studio Code](https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code)

## My Installed Extensions

- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
- [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)
- [C#](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp)
- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [Git Extension Pack](https://marketplace.visualstudio.com/items?itemName=donjayamanne.git-extension-pack)
  - [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)
  - [gitignore](https://marketplace.visualstudio.com/items?itemName=codezombiech.gitignore)
  - [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
  - [Open in Github / Bitbucket / VisualStudio.com](https://marketplace.visualstudio.com/items?itemName=ziyasal.vscode-open-in-github)
  - [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)
- [Git Project Manager](https://marketplace.visualstudio.com/items?itemName=felipecaputo.git-project-manager)
- [Github Markdown Preview](https://marketplace.visualstudio.com/items?itemName=bierner.github-markdown-preview)
  - [Markdown Checkboxes](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-checkbox)
  - [Markdown Emoji](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-emoji)
  - [Markdown Preview Github Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles)
  - [Markdown yaml Preamble](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-yaml-preamble)
- [Live Share Extension Pack](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
  - [Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)
  - [Live Share Audio](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-audio)
  - [Live Share Chat](https://marketplace.visualstudio.com/items?itemName=karigari.chat)
  - [Peocock](https://marketplace.visualstudio.com/items?itemName=johnpapa.vscode-peacock)
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf)
- [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)
- [Matlab](https://marketplace.visualstudio.com/items?itemName=Gimly81.matlab)
- [Modern VHDL](https://marketplace.visualstudio.com/items?itemName=rjyoung.vscode-modern-vhdl-support)
- [Python Extension Pack](https://marketplace.visualstudio.com/items?itemName=donjayamanne.python-extension-pack)
  - [Django](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django)
  - [Jinja](https://marketplace.visualstudio.com/items?itemName=wholroyd.jinja)
  - [MagicPython](https://marketplace.visualstudio.com/items?itemName=magicstack.MagicPython)
  - [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
  - [Visual Studio IntelliCode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
- [Remote - WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl) (Windows only)
- [reStructuredText](https://marketplace.visualstudio.com/items?itemName=lextudio.restructuredtext)
- [Tcl](https://marketplace.visualstudio.com/items?itemName=bitwisecook.tcl)
- [TSLint](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-typescript-tslint-plugin)
- [Verilog HDL/SystemVerilog](https://marketplace.visualstudio.com/items?itemName=mshr-h.VerilogHDL)
- [VSCode Great Icons](https://marketplace.visualstudio.com/items?itemName=emmanuelbeziat.vscode-great-icons)
- [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
- [VSNotes](https://marketplace.visualstudio.com/items?itemName=patricklee.vsnotes)

## VS Code Configuration

These settings are configured in the `settings.json` file.

add [Vertical rulers in Visual Studio Code?][Cfg1]

    "editor.rulers": [80,120],

add [File associations in vscode][Cfg2] for Alter/Intel Quartus files (.qsf,
.qpf) and constraint files (.sdc, .xdc) for Alter/Intel and Xilinx.

    "files.associations": {
        "*.qsf" : "tcl",
        "*.qpf" : "tcl",
        "*.sdc" : "tcl",
        "*.xdc" : "tcl"
    },

configure some paths for extensions

    "matlab.mlintpath": "c:\\<Matlab Path>\\bin\\win64\\mlint.exe",
    "markdown-pdf.executablePath" : "C:\\<Chrome Path>\\chrome.exe"

[Cfg1]: https://stackoverflow.com/questions/29968499/vertical-rulers-in-visual-studio-code
[Cfg2]: https://stackoverflow.com/questions/30369258/file-associations-in-vscode#30421000

## Extension Development

- [Extension API](https://code.visualstudio.com/api)
  - [Your First Extension](https://code.visualstudio.com/api/get-started/your-first-extension)
  - [Extension Guides](https://code.visualstudio.com/api/extension-guides/overview)
  - [Language Extension Overview](https://code.visualstudio.com/api/language-extensions/overview)
- [Testing your VS Code extensions](https://vscode.rocks/testing/)

### JavaScript

- [W3Schools Online Web Tutorials](https://www.w3schools.com/)
  - [JavaScript Tutorial](https://www.w3schools.com/js/default.asp)
- [The Modern JavaScript Tutorial](https://javascript.info/)
- [JavaScrip - Learn web development](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
  - [Asynchronous JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous)

### TypeScript

- [TypeScript in Visual Studio Code](https://code.visualstudio.com/Docs/languages/typescript)
- [TypeScript tutorial in Visual Studio Code](https://code.visualstudio.com/docs/typescript/typescript-tutorial)
- [Typescript - Javascript that scales.](https://www.typescriptlang.org/)
- [TypeScript Deep Dive](https://basarat.gitbooks.io/typescript/)

## Node.js

- [How to Create and Publish Your First Node.js Module](https://codeburst.io/how-to-create-and-publish-your-first-node-js-module-444e7585b738)

### Language Syntax Parsing

- [VS Code - TextMate grammars](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide#textmate-grammars)
  - [TextMate - Language Grammars](https://macromates.com/manual/en/language_grammars)
- [VS Code - Using YAML to write a grammar](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide#using-yaml-to-write-a-grammar)
  - [The Official YAML Web Site](https://yaml.org/)
    - [YAML Reference Card](https://yaml.org/refcard.html)

### Language Server Extension

- [Language Server Extension Guide](https://code.visualstudio.com/api/language-extensions/language-server-extension-guide)
- [Language Server Protocol (LSP)](https://microsoft.github.io/language-server-protocol/)
- [Language Server Protocol GIT Repo](https://github.com/Microsoft/language-server-protocol)
