# EEx Formatter/Beautify

Most of solutions that exist on the Internet tell you to create a task and call it from the ctrl-shift-p menu.

This extension basically uses [htmlbeautifier](https://github.com/threedaymonk/htmlbeautifier) to format your file using the Formatter API from vscode, so no need to create a hack using Task, etc.

## Features

![Demo GIF](https://raw.githubusercontent.com/zerokol/vscode-eex-beautify/master/images/demo.gif)

## Requirements

```
gem install htmlbeautifier
```

NOTE: Filenames with extension `.html.eex` might be recognized as an `html` file, not as an `eex` file. In that case, add a setting in your `settings.json` like below:

```json
"files.associations": {
  "*.eex": "eex"
}
```

## Settings

| Setting                              | Description                                           | Default |
| ------------------------------------ | ----------------------------------------------------- | ------- |
| `vscode-eex-beautify.tabStops`       | Set number of spaces per indent                       | 2       |
| `vscode-eex-beautify.tab`            | Indent using tabs                                     | false   |
| `vscode-eex-beautify.indentBy`       | Indent the output by NUMBER steps                     | 0       |
| `vscode-eex-beautify.stopOnErrors`   | Stop when invalid nesting is encountered in the input | false   |
| `vscode-eex-beautify.keepBlankLines` | Set number of consecutive blank lines                 | 0       |

## References

[Base Idea](https://github.com/aliariff/vscode-erb-beautify)
