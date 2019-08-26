# Visual Studio Code for Visual Basic

![Visual Studio Marketplace Version](https://img.shields.io/visual-studio-marketplace/v/aferri.avb?color=brightgreen&label=version&logo=visual-studio-code)
![Visual Studio Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/aferri.avb?color=blueviolet&label=installs&logo=visual-studio-code)
![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/aferri.avb?color=blue&label=downloads&logo=visual-studio-code)
![Visual Studio Marketplace Rating](https://img.shields.io/visual-studio-marketplace/r/aferri.avb?color=yellow&label=rating&logo=visual-studio-code)

## Legend
- [Contributors](#contributors)
- [Changelog](#changelog)
- [Syntax Highlighting](#syntax-highlighting)
- [Snippets](#snippets)
- [Basic code](#basic-code)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Contacts](#contacts)
- [Links](#links)
- [Handy links](#handy-links)


## Contributors

### This is a fork of the repository provided by [spences10](https://github.com/spences10)!
All credits goes to this amazing guy.


## Changelog

- Added snippet for add a variable with custom type.


## Syntax Highlighting

This package provides syntax highlighting and snippets for visual basic.

All are based on an import of the [VBScript.tmLanguage](https://github.com/SublimeText/VBScript/blob/master/VBScript.tmLanguage)
file from the [Sublime Text VBScript](https://github.com/SublimeText/VBScript) repository.


## Snippets

### Basic code
- Variables declaration (ex. **dim var_name as boolean**)
- Variables declaration with inline instantiation
- Operators (if, else, for ecc)
- Subroutine/Function declaration with or without error handling

## Usage

Start typing what you want to insert and suggestion should raise:

### Variables declaration

Type the variable type:

```vb
dim var_name as boolean  ' by typing bool
dim var_name as integer  ' by typing int
dim var_name as string   ' by typing string

dim var_name as type     ' by typing type
```

For private or public declaration type **p** or **pu** before the type:

```vb
private var_name as boolean  ' by typing pbool
public var_name as boolean   ' by typing pubool

private var_name as integer  ' by typing pint
public var_name as integer   ' by typing puint

private var_name as type     ' by typing ptype
public var_name as type      ' by typing putype
```

For declaration with inline assignment type **a** before the type:

```vb
dim var_name as boolean: var_name = value  ' by typing abool
dim var_name as integer: var_name = value  ' by typing aint

dim var_name as type: var_name = value     ' by typing atype
```

### Subroutine and functions

Type **sub** or **func** for a standard private method:

```vb
' by typing sub
private sub sub_name()
end sub

' by typing func
private function function_name()
end function
```

For public prepend **p**:

```vb
' by typing psub
public sub sub_name()
    ' Add something here
end sub

' by typing pfunc
public function function_name() as boolean  ' Return type will be asked when inserting the snippet
    ' Add something here
    function_name = true
end function
```

For method with try-catch add **e** at the end:

```vb
' by typing sube
private sub sub_name()
    on error goto ErrorHandler

    ' Add something here

    on error goto 0
    exit sub
ErrorHandler:
    ' Handle the exception
end sub

' by typing pfunce ('p' for public, 'func' for function, and 'e' for add error handling)
public function function_name() as boolean  ' Return type will be asked when inserting the snippet
    on error goto ErrorHandler

    ' Add something here
    function_name = true

    on error goto 0
    exit function
ErrorHandler:
    ' Handle the exception
end function
```

### Utilities

Insert a file header (XCode style):

```vb
' by typing header
'
' file_name
' current_path
'
' Created by author on current_date.
' Modified by contributor on current_date.
' Copyright © company 2019. All rights reserved.
'
```
- file_name: automatically inserted.
- current_path: automatically inserted.
- current_date: automatically inserted, only creation date is asked if you need to change it.

Print to output console:

```vb
' by typing print
debug.print var_name

' by typing prints
debug.print "string"
```

## Installation

Launch vscode and press [ctrl + p], paste the command below, and press enter.

```
$ ext install avb
```

## Contributing

Please fork this repository and contribute back using pull requests.

Any contributions, large or small, major features, bugfixes and
integration tests are welcomed and appreciated but will be thoroughly
reviewed and discussed.

## Contacts

You can contact me in the following ways:
- Mail: [alessio.ferri20@gmail.com](mailto:alessio.ferri20@gmail.com)
- Github: [aferri](https://github.com/aferri-alstom)

Original contributor details:
- Mail: [spences10apps@gmail.com](mailto:spences10apps@gmail.com)
- Github: [spences10](https://github.com/spences10)

## Links

- [Source](https://github.com/aferri-alstom/vscode-vba)
- [Marketplace](https://marketplace.visualstudio.com/items?itemName=aferri.avb)

Original contributor details:
- [Source](https://github.com/spences10/vscode-vba)
- [Marketplace](https://marketplace.visualstudio.com/items?itemName=spences10.VBA)

## Handy links

Some good documentation on the CLI:

https://vscode-docs.readthedocs.io/en/latest/tools/vscecli/
