# Visual Studio Code for Visual Basic

[![Marketplace Version](https://vsmarketplacebadge.apphb.com/version/aferri.avb.svg)](https://marketplace.visualstudio.com/items?itemName=aferri.avb)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/aferri.avb.svg)](https://marketplace.visualstudio.com/items?itemName=aferri.avb)
[![Rating](https://vsmarketplacebadge.apphb.com/rating/aferri.avb.svg)](https://marketplace.visualstudio.com/items?itemName=aferri.avb)

<!-- TOC depthFrom:2 -->

- [Syntax Highlighting](#syntax-highlighting)
- [Snippets](#snippets)
- [Basic code](#basic-code)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Contacts](#contacts)
- [Links](#links)
- [Handy links](#handy-links)

<!-- /TOC -->

## Fork repository of spences10

This repo is a fork of the one published by spences10, all credits goes to him.

## Syntax Highlighting

This package provides syntax highlighting and snippets for visual basic.

Based off an import of the
[VBScript.tmLanguage](https://github.com/SublimeText/VBScript/blob/master/VBScript.tmLanguage)
file from the
[Sublime Text VBScript](https://github.com/SublimeText/VBScript)
repository.

## Snippets

### Basic code

- Variables declaration (dim/private/public var_name as type)
- Variables declaration with inline instantiation
- Operators (if, else, for ecc)
- Subroutine/Function declaration with or without error handling

### Usage

start typing what you want to insert and suggestion should raise:

### Variables declaration

Type the variable type:

```
bool   --> dim var_name as boolean
int    --> dim var_name as integer
string --> dim var_name as string
```

For private or public declaration type 'p' or 'pu' before the type:

```
pbool  --> private var_name as boolean
pubool --> public var_name as boolean
```

For declaration with inline assignment type 'a' before the type:

```
abool --> dim var_name as boolean: var_name = value
```

## Installation

Launch vscode and press [ctrl + p], paste the command below, and press enter.

```
ext install avb
```

## Contributing

Please fork this repository and contribute back using pull requests.

Any contributions, large or small, major features, bugfixes and
integration tests are welcomed and appreciated but will be thoroughly
reviewed and discussed.

## Contacts

You can contact me in the following ways:

- Mail : [spences10apps@gmail.com](mailto:spences10apps@gmail.com)
- Github : [spences10](https://github.com/spences10)

## Links

- [Source Code](https://github.com/spences10/vscode-vba)
- [Market](https://marketplace.visualstudio.com/items?itemName=spences10.VBA)

## Handy links

Some good documentation on the CLI:

https://vscode-docs.readthedocs.io/en/latest/tools/vscecli/
