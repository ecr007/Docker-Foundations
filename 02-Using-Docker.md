# Using Docker

How do navigate Docker CLI?

```docker --help```

**Top level command with sub commands underneath it**

```docker network --help``
```docker network create --help```

Each command within docker CLI support --help flag.

## Create a Docker Container

There are two way to create Docker containers, the long way and the short way.

Containers are created from container images, container images are compressed and pre-packege file system that contain, no pun intended, your apps along with its environement and configuration with an instructions on how to start your applications. That instruction is called the entry point.  

```docker container create hello-world:linux```

```docker container create [options] IMAGE [command] [args...]```

Note: ":linux" has installed the linux version of hello-world docker container.

Note: docker container create does not run the container only creating it. 

Note: Every container by docker has a container ID, this makes it easy to inspect and interact with them. 

**How to see the docker container has been running ?**

```docker ps```
```docker ps --all``` : to show all container 

**How to start docker container**

```docker container start CONTAINER ID``` 

After start a container is important to see the STATUS => Exited (0) othewise it is a error.

**Logs**

```docker logs [FIRST THREE CHARACTERS OF CONTAINER ID]```

**How to start a docker container with logs activated**

```docker container start --attach [CONTAINER ID]```



