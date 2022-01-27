Xentu Lua Snippets for VS Code
======

This extension provides code snippets for the Xentu game engine for use in VS Code.
Supports keywords, properties, functions, and also constants for things like Keyboard & Mouse.

Some features are not yet added, such as class properties and functions, these will be provided soon. For now now refer to the documentation if you get stuck, found at https://docs.xentu.net

This package is part of the Xentu game engine project: https://xentu.net

```
```

Running a Xentu game from VS Code
----

If you have the Xentu SDK installed, you can enhance your coding experience by
adding a few shortcuts to your editor. With your game folder open in VS Code,
navigate to the Terminal menu, and select `"Configure Default Build Task..."`

When prompted select `"Create task.json from template"` then choose `"Others"`.

This will create a file called *'.vscode\tasks.json`* to which you could modify to
look similar to this:

```json
{
    // See https://go.microsoft.com/fwlink/?LinkId=733558
    // for the documentation about the tasks.json format
    "version": "2.0.0",
    "tasks": [
        {
            "label": "Run Game",
            "type": "shell",
            "command": "xentu .",
            "problemMatcher": [],
            "group": {
                "kind": "build",
                "isDefault": true
            }
        }
    ]
}
```

After that a new command called `"Run Game"` will be added to VS Code. And to use it, all we need to do is use the keyboard shortcut
`CTRL+SHIFT+B`.

Happy coding!