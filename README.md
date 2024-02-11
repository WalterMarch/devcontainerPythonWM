# python-devcon - Visual Studio Code devcontainer for Python

## Sample Dev Container file(s) for Python in VS Code Containerized Development

*assumptions*: Docker and VS Code installed as well as the Dev Containers extension for Visual Studio Code.

*usage*: clone the repo then open in Visual Studio Code.

*example*:  clone the repo; open a new VS Code window; open the directory containing this repo; when prompted, choose Reopen in Container. 

I chose to use a Ubuntu base and install `pyenv` to allow multiple version of Python.

Based on https://code.visualstudio.com/docs/devcontainers/containers

Jumping off point for `pyenv`: https://realpython.com/intro-to-pyenv/

## Run the Sample Code

In the `/workspaces/devcontainer-python` directory, run this command:

```bash
python3 sample/hello_world.py
```

### miscellany

`configit.sh` looks like this:

```bash
#!/bin/bash

git config --global user.email "yourEmail@mail.com"
git config --global user.name "yourGitUserName"
git config --global push.autoSetupRemote true

git config --global --add safe.directory $1
```
