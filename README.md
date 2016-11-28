# EJS 2

EJS syntax definition for Sublime Text 3. Works with [EJS v2](http://ejs.co/) syntax. Also includes EJS tag autocompletion and some snippets.

> Requires Sublime Text 3 build >=3103

## Installation

Use [Package Control](https://packagecontrol.io/docs/usage) to install [**EJS 2**](https://packagecontrol.io/packages/EJS%202).

#### Setting the default syntax

By default, files with the extension `.ejs` are opened with the `EJS (<% %>)` syntax.

If you'd like to open files with a different extension as EJS or you want to use delimiters other than `<% %>`, follow these steps to set the default EJS syntax for an extension:

1. Open an EJS file
2. Select `View` from the menu
3. Then `Syntax` &rarr; `Open all with current extension as...` &rarr; `EJS 2` &rarr; `EJS (<delimiter>)`
4. Repeat this for each extension you want to open as EJS

This package includes syntax definitions for the following additional delimiters: `<? ?>`, `<$ $>`, `<@ @>`.

#### Color Scheme

`EJS 2` comes with the `Dracula EJS` color scheme, which is a modified version of [zertosh/dracula-theme](https://github.com/zertosh/dracula-theme/tree/dark). You can select it from: `Preferences` &rarr; `Color Scheme` &rarr; `EJS 2`.

[`Oceanic Next`](https://github.com/voronianski/oceanic-next-color-scheme) is also a good color scheme for EJS that works right out of the box.

If you'd prefer to use a different color scheme, you may need to add lines like [these](https://github.com/nwoltman/sublime-ejs/blob/master/Dracula%20EJS.YAML-tmTheme#L228-241) to make the highlighting more compatible with EJS.

#### Example (with *Dracula EJS*)

![](example.png)

#### Snippets

In the HTML scope:

+ `if`+`TAB` - Inserts EJS `if` statement
+ `for`+`TAB` - Inserts EJS `for` loop

### Highlighting Hiccup

Currently, this syntax definition cannot recognize when an EJS closing tag (i.e. `%>`) is part of a JavaScript string or regex, so it will end the JavaScript section and return to highlighting HTML even though it shouldn't.

Example:

```js
<%
const str = 'These are EJS delimiters: <% %>';
// Now right here is HTML because of this ^^
%>
```

However, you can get around this without changing the meaning of your JavaScript code by adding a backslash (`\`) before the closing `>` like so:

```js
<%
const str = 'These are EJS delimiters: <% %\>';
// Everything is fine here
%>
```

## Contributing

Most problems are best addressed by opening an [issue](https://github.com/nwoltman/sublime-ejs/issues).
<!-- Also, check out the [contributing guide](https://github.com/nwoltman/sublime-ejs/blob/master/CONTRIBUTING.md). -->
