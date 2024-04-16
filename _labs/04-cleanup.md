---
layout: lab
number: 4
title:  "Cleanup"
---

### Goals
Learn to view and name docker containers and clean them up.

## View Your Containers

Docker comes with a command to view the containers that are currently running on
your system. Let's try it now.

## Name Your Containers

In lab 03, we used names to help us keep track of our containers. Let's learn
more about that now.

By passing `--name my-container`, we ask Docker to use the name we specify
rather than making up it's own. This can be useful to help you keep track of the
different containers you've run.

Even though that container exited immediately, the container still exists on
your system (as discussed in the previous lab). Because of that, you can't
re-use the same name again.

This is an error you might see somewhat frequently if you start using named
containers and forget to clean them up. Let's learn how to fix it.

## Clean Up Your Containers

Yep, when a docker container exits, it hangs around on your system until you
clean it up. This can be really handy for debugging, but we’re done with these
containers for now. Let's remove some of them. You can remove them by ID or by
name. Let's remove `my-container`, along with several others we created in
previous labs but don't need anymore. Note that **your IDs will be different
than mine**!

It is perfectly safe to remove any container listed by `docker ps -a` that you
don't want to restart - we won’t need them anymore. In the future, you might see
us pass the `--rm` flag to `docker run`. That option automatically removes a
container when we’re finished with it so we don’t have to clean it up later.

Newer versions of Docker include a command called `docker system prune` that can
help you clean up a large number of stale containers and images from your
system. We'll discuss this in more depth later.
