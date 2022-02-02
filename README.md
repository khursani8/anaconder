## Persistent Anaconda environment in docker

I use it for windows pc because I want to play game and do deeplearning in this pc
Tested on Windows 11 with WSL2 enabled

How to use:
1. install docker for Windows
2. docker-compose up -d
3. docker ps
4. docker ps -l -q # get the container id
5. docker exec -it 'put container id here' bash