## Flutter - Dev Notes

### Starting the Android emulator from CLI

Use the following commands to start the Android emulator (one of your AVD devices) from the command line, without having to start Android Studio:

```bash
$ ~/Library/Android/sdk/tools/bin/avdmanager list avd        // To list the existing virtual devices.
$ ~/Library/Android/sdk/tools/emulator -avd Nexus_5_API_27   // Start the device having that name.
```

### VSCode settings

The following settings were added in Visual Studio Code:
- having the status bar background with the same color as the theme (Material Theme Ocean), instead of the default orange color using:
  ``json
  "workbench.colorCustomizations": {
    "statusBar.debuggingBackground": "#263238",
  }
  ```
- disabling the "fake" closing parens comments using `"dart.closingLabels": false`
- increased the allowed length of the line (considered by `dartfmt`) using `"dart.lineLength": 110`

