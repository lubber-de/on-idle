# On Idle

This a very simple extension that triggers configurable commands after a period of inactivity, i.e. when you stop typing.

When commands are configured for current file extension, a button is displayed in the status bar (a watch with a tick or a cross next to it) indicating if **On Idle** is enabled for that file extension:

<img src="https://raw.githubusercontent.com/Gruntfuggly/on-idle/master/button.png">

Click the button to disable or enable.

## Configuration

`onIdle.commands` specifies the commands to trigger for specific file extensions.

Example:
```javascript
onIdle.commands: {
    "md": {
        "enabled": true,
        "commands:" [
            "markdown-latex-toggle.markdown-to-latex"
        ]
    }
}
```

Use `onIdle.delay` to change the delay after which the commands are triggered. The value is specified in milliseconds. The default delay is 1 second.

The position of the status bar button can be configured using `onIdle.buttonAlignment` and `onIdle.buttonPriority`. The icon itself can be changed with `onIdle.buttonIcon`.

## Installing

You can install the latest version of the extension via the Visual Studio Marketplace [here](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.on-idle).

### Source Code

The source code is available on GitHub [here](https://github.com/Gruntfuggly/on-idle).

## Credits

Extension icon made by <a href="http://www.freepik.com" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a>
