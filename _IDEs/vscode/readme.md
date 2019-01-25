## VS Code

The settings that I am using in Visual Studio Code:

- Status bar background color in debug mode to be the quite the same as the theme that I am currently like (Pines),:
  ```json
  "workbench.colorCustomizations": {
    "statusBar.debuggingBackground": "#263238",
  }
  ```
- Disabled the "fake" closing parens comments using:
  ```json
  "dart.closingLabels": false
  ```
- Increased the allowed length of the line (considered by `dartfmt`) using:
  ```json
  "dart.lineLength": 100
  ```
- Default values used by Flutter generator:
  ```json
  "dart.flutterCreateIOSLanguage": "swift",
  "dart.flutterCreateOrganization": "tech.vision8",
  ```
- Handy keyboard shortcuts:
  - General ones:
    - `cmd + alt + 1` for Explorer view
    - `cmd + alt + 2` for Search view
    - `cmd + alt + 4` for Debug view
    - `cmd + alt + d` for Debug console
  - IDEA like ones:
    - `cmd + y` for deleting the current line
    - `cmd + d` for duplicating the current line
  
  The concrete settings as stored in `keybindings.json`:
  ```json
  [
    {
        "key": "alt+cmd+1",
        "command": "workbench.view.explorer"
    },
    {
        "key": "alt+cmd+2",
        "command": "workbench.view.search"
    },
    {
        "key": "alt+cmd+4",
        "command": "workbench.view.debug"
    },
    {
        "key": "alt+cmd+d",
        "command": "workbench.debug.action.toggleRepl"
    },
    {
        "key": "cmd+d",
        "command": "editor.action.copyLinesDownAction",
        "when": "editorTextFocus && !editorReadonly"
    },
    {
        "key": "cmd+y",
        "command": "editor.action.deleteLines",
        "when": "textInputFocus && !editorReadonly"
    },
  ]
  ```

