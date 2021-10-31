# Learn NLP
NLP Specialisation with DeepLearning.ai


## dev container

The work in this workspace is done inside a dev container, this allows my to set up the python envinronment with the needed configuration without interfering with local setup, and the devcontainer definition is portbale to run on other machines.

Vscode can create docker containers as dev envinronments. To use dev containers in VSCode, run the command `Remote-Containers: Add Development Container Configuration Files...`.


reference: <https://code.visualstudio.com/docs/remote/create-dev-container>


## attaching to running container from terminal


list running containers:
```
docker container list
```

output:
```
CONTAINER ID   IMAGE                                           COMMAND                  CREATED        STATUS        PORTS      NAMES
e6aef40a0ff3   vsc-learnnlp-9f54613aa2c9c2c2dba68c3fbe9146b0   "tini -g -- start-no…"   45 hours ago   Up 45 hours   8888/tcp   recursing_dubinsky
```

attach to container:
```
docker exec -it e6aef40a0ff3 bash
```

press `Ctrl p q` to detach.
