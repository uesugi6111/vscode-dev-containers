# PowerShell

## Summary

*Develop PowerShell scripts without installing anything locally.*

| Metadata | Value |  
|----------|-------|
| *Contributors* | The VS Code Team |
| *Definition type* | Dockerfile |
| *Published images* | mcr.microsoft.com/vscode/devcontainers/powershell |
| *Available image variants* | 6, 7 |
| *Published image architecture(s)* | x86-64 |
| *Works in Codespaces* | Yes |
| *Container host OS support* | Linux, macOS, Windows |
| *Languages, platforms* | PowerShell |


## Using this definition with an existing folder

While this definition should work unmodified, you can select the version of PowerShell the container uses by updating the `VARIANT` arg in the included `devcontainer.json` (and rebuilding if you've already created the container).

```json
"args": { "VARIANT": "7" }
```

You can also directly reference pre-built versions of `.devcontainer/base.Dockerfile` by using the `image` property in `.devcontainer/devcontainer.json` or updating the `FROM` statement in your own  `Dockerfile` to one of the following. An example `Dockerfile` is included in this repository.

- `mcr.microsoft.com/vscode/devcontainers/powershell` (latest)
- `mcr.microsoft.com/vscode/devcontainers/powershell:6`
- `mcr.microsoft.com/vscode/devcontainers/powershell:7`

Version specific tags tied to [releases in this repository](https://github.com/microsoft/vscode-dev-containers/releases) are also available.

- `mcr.microsoft.com/vscode/devcontainers/powershell:0-6`
- `mcr.microsoft.com/vscode/devcontainers/powershell:0.135-6`
- `mcr.microsoft.com/vscode/devcontainers/powershell:0.135.0-6`

Alternatively, you can use the contents of `base.Dockerfile` to fully customize your container's contents or to build it for a container host architecture not supported by the image.

### Adding the definition to your folder

This definition does not require any special steps to use. Just follow these steps:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.

2. To use VS Code's copy of this definition:
   1. Start VS Code and open your project folder.
   2. Press <kbd>F1</kbd> select and **Remote-Containers: Add Development Container Configuration Files...** from the command palette.
   3. Select the PowerShell definition.

3. To use latest-and-greatest copy of this definition from the repository:
   1. Clone this repository.
   2. Copy the contents of `containers/powershell/.devcontainer` to the root of your project folder.
   3. Start VS Code and open your project folder.

4. After following step 2 or 3, the contents of the `.devcontainer` folder in your project can be adapted to meet your needs.

5. Finally, press <kbd>F1</kbd> and run **Remote-Containers: Reopen Folder in Container** to start using the definition.

## Testing the definition

This definition includes some test code that will help you verify it is working as expected on your system. Follow these steps:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started) to set up your machine.
2. Clone this repository.
3. Start VS Code, press <kbd>F1</kbd>, and select **Remote-Containers: Open Folder in Container...**
4. Select the `containers/powershell` folder.
5. After the folder has opened in the container, press <kbd>F5</kbd> to start the project.
6. You should see "Hello remote world #1!" up to 100 in a terminal window after the program executes.
7. From here, you can add breakpoints or edit the contents of the `test-project` folder to do further testing.

## License

Copyright (c) Microsoft Corporation. All rights reserved.

Licensed under the MIT License. See [LICENSE](https://github.com/Microsoft/vscode-dev-containers/blob/master/LICENSE).