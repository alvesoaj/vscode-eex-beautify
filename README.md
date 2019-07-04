# EEX Formatter/Beautify

Most of solution that exist in the internet is tell you to create a task and call it using ctrl-shift-p menu.

This extension basically using [htmlbeautifier](https://github.com/threedaymonk/htmlbeautifier) to format your file using the Formatter API from the vscode, so no need to create a hack using Task, etc.

## Features

TODO

## Requirements

```
gem install htmlbeautifier
```

NOTE: For you that have a filename with extension `.html.eex`, your file might be recognized as `html` file, not as `eex` file. In that case, add a setting in your `settings.json` like below:

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
