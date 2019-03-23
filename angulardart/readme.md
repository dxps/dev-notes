## AngularDart - Notes


#### Windows specifics

Installed by extracting the Dart SDK archive file ver 2.2.0 for Windows x64.

Created `DART_HOME` env var, and added to `PATH` the following entries:
* `%DART_HOME%\bin`
*  `c:\Users\stduser\AppData\Roaming\Pub\Cache\bin`

For listening on a different port (as in many cases the default :8080 is being used by an antivirus program) use:
```
webdev serve web:8888
...
Serving `web` on http://localhost:8888
```
