# Symbols & Outline Tree View

- [Outline View - June 2018](https://code.visualstudio.com/updates/v1_25#_outline-view)
  - [DocumentSymbols](https://code.visualstudio.com/updates/v1_25#_document-symbols)
- [VS Code - User Interface](https://code.visualstudio.com/docs/getstarted/userinterface)
  - [Go to Symbol](https://code.visualstudio.com/docs/editor/editingevolved#_go-to-symbol)
- [VS Code Documentation](https://vscode.readthedocs.io/en/latest/)
  - [Language Extension Guidelines](https://vscode.readthedocs.io/en/latest/extensionAPI/language-support/)

source code:

- [VS Code - Github](https://github.com/Microsoft/vscode)
  - [vscode/src/vs/vscode.d.ts](https://github.com/Microsoft/vscode/blob/master/src/vs/vscode.d.ts)

## VS Code source code for Symbols & Outline View

- [Markdown support](https://github.com/microsoft/vscode/tree/34ba2e2fbfd196e2d6db5a4db0e42d03a97c655e/extensions/markdown-language-features)
  - [vscode/extensions/markdown-language-features/src/features/documentSymbolProvider.ts](https://github.com/microsoft/vscode/blob/34ba2e2fbfd196e2d6db5a4db0e42d03a97c655e/extensions/markdown-language-features/src/features/documentSymbolProvider.ts)
  - [vscode/extensions/markdown-language-features/src/features/documentLinkProvider.ts](https://github.com/Microsoft/vscode/blob/34ba2e2fbfd196e2d6db5a4db0e42d03a97c655e/extensions/markdown-language-features/src/features/documentLinkProvider.ts)

## LSP Code for Symbols & Outline View

- [DocumentSymbol[]](https://microsoft.github.io//language-server-protocol/specifications/specification-3-14/#textDocument_documentSymbol)

## Other Extensions using Symbols & Outline View

- [perl-outline](https://marketplace.visualstudio.com/items?itemName=hitode909.perl-outline)
  - [vscode-perl-outline](https://github.com/hitode909/vscode-perl-outline)
    - [vscode-perl-outline/src/documentSymbolProvider.ts](https://github.com/hitode909/vscode-perl-outline/blob/master/src/documentSymbolProvider.ts)
- [Fortran](https://marketplace.visualstudio.com/items?itemName=Gimly81.fortran)
  - [vscode-fortran](https://github.com/Gimly/vscode-fortran)
    - [vscode-fortran/src/documentSymbolProvider.ts](https://github.com/Gimly/vscode-fortran/blob/229cddce53a2ea0b93032619efeef26376cd0d2c/src/documentSymbolProvider.ts)

Alternative Tree View:

- [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)
  - [todo-tree](https://github.com/Gruntfuggly/todo-tree)

## Suggested Extensions

- [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
- [npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script)
