# ``sandbox.javadev``
- Author: Marcel Nika



## 🔧 1. Prerequisites

- [Docker](https://www.docker.com/get-started) installed and running
- [Visual Studio Code](https://code.visualstudio.com/)
- Extension: **Remote - Containers** (`ms-vscode.remote-containers`)



## ⚙️ 2. Clone the repository

### Either via ``HTTP``

````bash
$ git clone https://github.com/mnka02/sandbox.javadev.git
````

### Or via ``SSH``

````bash
$ git clone git@github.com:mnka02/sandbox.javadev.git
````



## 🔍 3. Optional Modifications

- [Modify Container Name](docker-compose.yml)

  ````yaml
  container_name: devSandbox.java
  ````

- [Modify Port](docker-compose.yml)

  ````yaml
  ports:
  	- "5005:5005"
  ````

- [Modifiy list of ``VSCode`` -Extensions](.devcontainer/devcontainer.json)

  ````json
  "extensions": [
          "vscjava.vscode-java-pack",
          "ms-vscode.remote-containers",
          "eamodio.gitlens"
    			// add id of extension here
  ]
  ````

  

## 🚀 4. Start the Dev Container

1. Open the project in VS Code.
2. Open the **Command Palette** (`F1` or `Ctrl+Shift+P`)
3. Select: `Remote-Containers: Reopen in Container`



## ✅ You're Ready!

You now have a fully working Java/Maven development environment in a container with:

- Maven & JDK 17
- Debugging support (port 5005)
- VS Code integration with IntelliSense and extensions
