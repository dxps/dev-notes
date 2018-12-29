## Flutter - Dev Notes

### Starting the Android emulator from CLI

Use the following commands to start the Android emulator (one of your AVD devices) from the command line, without having to start Android Studio:

```bash
$ ~/Library/Android/sdk/tools/bin/avdmanager list avd        // To list the existing virtual devices.
$ ~/Library/Android/sdk/tools/emulator -avd Nexus_5_API_27   // Start the device having that name.
```
