
# Instructions for setting up your development environment with Docker  

The files for setting up the docker environment in VSCode are locatted in the *.devcontainer* and *.vscode* folders. The docker image gets pulled from the following [DockerHub location](https://hub.docker.com/r/robertinoiog/plutus-pioneer-program-4). 

In case you do not want to use a Docker integration inside VSCode editor you can use the Docker image directly. The *Dockerfile* that contains the instructions for building an image is located inside the *.devcontainer* folder. 

In both cases you will need to install [Docker Desktop](https://docs.docker.com/get-docker/). It is recomended to install and run Docker Desktop on your native OS. If you want to run Docker Desktop inside a Virtual Machine read through [these notes](https://docs.docker.com/desktop/vm-vdi/). 

The following instructions explain how to setup VSCode with Dcoker:
* Download and install VSCode from [here](https://code.visualstudio.com/). 
* You need to start the Docker Desktop application which will start the Docker daemon. 
* Open VSCode, click on the Manage icon in the bottom left corner and choose the Extensions option. 
* A window showing the Extensions Marketplace will appear on the left side of the VS Code UI. In the search box, type *remote development* and then install this extension whicht is is provided by Microsoft. 
* After successfully installing the Remote Development extension, you will note that an **Uninstall** button appears in the extension description tab. 
* Close VSCode, clone this repository to your computer, then open VSCode and in the File menu click Open Folder. Select the folder you have cloned with Git. 
* When VS Code opens, the Remote Development extension will detect the Docker container. You'll see a message asking to reopen your project in the container on the bottom right side. Click the **Reopen in Container** button to build the docker container. 
* You can click the Starting Dev Container message to view the log. The build may take some time. After a few minutes, you will see a message in the log saying *Start: Run in container*. This message indicates that the dev container is ready. 
* You can safely close this terminal window by clicking the trash can icon in the upper right corner of the terminal window. Now, open a new terminal window in VS Code by clicking the **Terminal** menu and then **New Terminal**. From the new terminal window you can run and build Plutus projects. 