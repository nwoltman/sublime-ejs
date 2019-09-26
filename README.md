# EJS 2

[EJS](http://ejs.co/) syntax definition for Sublime Text 3. Includes EJS tag autocompletion and snippets.

## Installation

Use [Package Control](https://packagecontrol.io/docs/usage) to install [**EJS 2**](https://packagecontrol.io/packages/EJS%202).

### Setting the default syntax

By default, files with the extension `.ejs` are opened with the `EJS (<% %>)` syntax.

To open files with a different extension as EJS, or to use delimiters other than `<% %>`, follow these steps to set the default EJS syntax for a file extension:

1. Open an EJS file
2. Select `View` from the menu bar
3. Then select: `Syntax` &rarr; `Open all with current extension as...` &rarr; `EJS 2` &rarr; `EJS (<delimiter>)`
4. Repeat for each extension you want to open as EJS

This package includes syntax definitions for the following additional delimiters: `<? ?>`, `<$ $>`, `<@ @>`.

### Color Scheme

`EJS 2` comes with the `Dracula EJS` color scheme, which is a modified version of [zertosh/dracula-theme](https://github.com/zertosh/dracula-theme/tree/dark). You can select it from: `Preferences` &rarr; `Color Scheme`.

[`Oceanic Next`](https://github.com/voronianski/oceanic-next-color-scheme) is also a good color scheme for EJS that works right out of the box.

If you'd prefer to use a different color scheme, you may need to add lines like [these](https://github.com/nwoltman/sublime-ejs/blob/a7cceaf26f3c3dd0ea4d64f9303c95d632f9d9e4/Dracula%20EJS.YAML-tmTheme#L273-L286) to make the highlighting more compatible with EJS.

#### Preview (with *Dracula EJS*)

![](example.png)

### Snippets

In the HTML scope:

+ `if`+`TAB` - Inserts EJS `if` statement
+ `for`+`TAB` - Inserts EJS `for` loop

## Contributing

Most problems are best addressed by opening an [issue](https://github.com/nwoltman/sublime-ejs/issues).
