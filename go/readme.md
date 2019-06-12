# GoLang related notes

## Running in debug mode in VSCode

In order to run the go app in VSCode, the well-known `delve` needs to be installed.
Here are the steps for macOS:
1. In the terminal, run `xcode-select --install`
2. Currently, running on macOS 10.14.5 (Mojave), go to `/Library/Developer/CommandLineTools/Packages/` and double-click on `macOS_SDK_headers_for_macOS_10.14.pkg`.
3. Clone `https://github.com/go-delve/delve` repo into `$GOPATH/src/github.com/go-delve` location.
4. In the terminal, cd that location and run `make install`.

Going back to VSCode, go to the Debug view and click the _play_ button to run. If no configuration exists, it will ask you first about the environment. Select _Go_ and the following `launch.json` file will be created:
```json
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Launch",
            "type": "go",
            "request": "launch",
            "mode": "auto",
            "program": "${fileDirname}",
            "env": {},
            "args": []
        }
    ]
}
```

Then you will be able to start the main package in debug mode.
<br/> <br/>


## Defining and Running my own tasks in VSCode

For defining my own commands, a `tasks.json` file needs to be created in `.vscode` folder that exists in the root of the project (example: `$GOPATH/src/<project-name>/.vscode`).
Here is an example that builds and run the app:

```json
{
    // See https://go.microsoft.com/fwlink/?LinkId=733558
    // for the documentation about the tasks.json format
    "version": "2.0.0",
    "tasks": [
        {
            "label": "Build and Run",
            "type": "shell",
            "command": "go build && ./hello",
            "group": {
                "kind": "build",
                "isDefault": true
            }
        }
    ]
}

```

Now, I can use Cmd+Shift+B to run it. Of course, multiple such tasks can be defined and the possible values for the group is either "build" or "test".


