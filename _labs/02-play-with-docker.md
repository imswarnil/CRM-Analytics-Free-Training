---
layout: lab
number: 2
title:  "Play With Docker"
---

### Goals
Learn to run basic commands with Docker and get to an interactive shell.

## Hello from Ubuntu

Let's run some simple commands in Docker. For this, we're going to use the
[Ubuntu](https://hub.docker.com/_/ubuntu/) Docker image, which will allow us to
run most Linux commands.

Let's break that down:

 - `docker run` is the Docker command to run a container.
 - `ubuntu` is the name of the Docker image we're running in our container. This
   image comes from Docker Hub.
 - `latest` is the “tag”, or version of the image that we want to use.
 - `echo "Hello from Ubuntu."` is the command that we're running inside the
   container.

Docker pulls the image for Ubuntu automatically if it isn't already cached. Then
it runs our echo command.

## Bash in Ubuntu

Instead of running `echo`, we can ask Docker to run `/bin/bash` inside the
Ubuntu container. This will get us to an interactive shell.

We are at a bash prompt! The prompt is `#` rather than `$`. This is a great way
to know that you’re at a prompt inside the Docker container rather than on your
host machine. (It also indicates that you’re the *root* user inside the
container \- more on that later). Let's run some simple commands and have a look
around.

Feel free to experiment some more inside the container, when you're done, run
`exit` to exit Bash and stop the container. Then move on to the next lab.
