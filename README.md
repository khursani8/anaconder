## Persistent Anaconda environment in docker

I use it for windows pc because I want to play game and do deeplearning in this pc without installing any dev stuff in my windows pc and I like to do work in ubuntu environment.
GPU work fine for me btw ;)

Tested on Windows 11 with WSL2 enabled

### How to use:
1. install docker for Windows
2. docker-compose up -d
3. docker ps
4. docker ps -l -q # get the container id
5. docker exec -it 'put container id here' bash

### Create new folder to sync
In docker-compose.yml under volumes can add your new folder "- ./src/:/home/src/:rw"

### Add new environment
Uncomment environment field and add your new environment variable

### open port
Add new port number under 'expose' field

### Increase shared memory
Change 'shm_size'

### Open folder in container using vscode
https://code.visualstudio.com/docs/remote/containers

### Attach container using vscode
https://code.visualstudio.com/docs/remote/attach-container