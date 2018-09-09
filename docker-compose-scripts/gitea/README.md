#INITIAL SETUP
You must have a git system user in order for gitea and docker to interact harmoniously. Run this cmd before initializing the gitea docker container for the first time, you only need to run this once.
```
$ sudo adduser --system --shell /bin/bash --gecos 'Git Version Control' --group --disabled-password --home /home/git git
```
Then you can run this in a screen session:
```
docker-compose --project-name gitea-app-test -f docker-compose.yml up
```
