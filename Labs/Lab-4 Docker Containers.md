# Lab 4 - Docker

## Objectives
This lab walks through the basics of docker images and containers

You must use Cloud9 for this lab since CloudShell does not support docker.

Notice that there is also a docker cheat sheet in the repository

## Part 1 - Exploring dockerspace 
```Console
$ docker image ls
$ docker container ls
$ docker network ls 
```

### Step 1-1 - Walkthrough
The instructor will walk through the example lab with you.

### Step 1-2 - Pulling and running images

```Console
$ docker run hello-world
$ docker pull ubuntu
$ docker run -it ubuntu /bin/bash
```

### Step 1-3 - Cleaning up
```Console
$ docker container ls -a
$ docker container prune
$ docker image ls
$ docker image rm ubuntu:latest
$ docker image rm hello-world:latest
```

---






