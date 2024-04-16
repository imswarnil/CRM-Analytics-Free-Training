---
layout: lab
number: 3
title:  "Container Persistence"
---

### Goals
Learn what happens when a container is stopped.

## Container Persistence

### Write a Text File

Inside a container, we can run commands just like any other Linux prompt. We can
also edit files.  Let's get back to a command prompt inside an Ubuntu container
and create a text file.

We were able to write to the filesystem inside the container. Cool. Let's go
back and look at that again.

Huh? What happened to our file? It isn't there anymore. This is happening
because we are in a different container than we were the first time. When we ran
the same `docker run` command, it started a _new_ container from the same Ubuntu
image. The filesystem inside the container is completely fresh - nothing is
shared with the first container we ran.

### Restart a Stopped Container

Can we get our file back? As a matter of fact, yes. We can get a list of all the
containers on our machine (including the stopped ones) with `docker ps -a`.


Because we restarted our stopped container instead of running a new container,
our changes to the filesystem were present. We can see the contents of the
`foo.txt` file that we made. With `docker start`, we can re-start a stopped
container. This can be useful for things like debugging, but is not a normal
part of the Docker workflow, so don't get used to using it too often.

Feel free to play around with the things we've learned so far to get comfortable
with them. When you're ready, move on to the next lab.
