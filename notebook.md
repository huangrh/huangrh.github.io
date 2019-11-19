# How to solve: vs code interactive windows slow too slow  

Essentially put this in your python.dataScience.runStartupCommands in setting.json

%config IPCompleter.use_jedi = False

ref: https://github.com/microsoft/vscode-python/issues/8171
