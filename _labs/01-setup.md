---
layout: lab
number: 1
title: "Setup"
description : Hello from Docker!This message shows that your installation appears to be working correctly
image : <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" fill="currentColor" class="w-16 h-16"><path d="M472,16H168a24,24,0,0,0-24,24V344a24,24,0,0,0,24,24H472a24,24,0,0,0,24-24V40A24,24,0,0,0,472,16Zm-8,320H176V48H464Z"></path><path d="M112,400V80H80V408a24,24,0,0,0,24,24H432V400Z"></path><path d="M48,464V144H16V472a24,24,0,0,0,24,24H368V464Z"></path></svg>
---

### Goals

To setup Docker on your machine.

## Install Docker

 {% include adsense.html type="article" %}

Install Docker CE for
[Windows](https://docs.docker.com/docker-for-windows/install/),
[Mac](https://docs.docker.com/docker-for-mac/install/), or
[Linux](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/) by
following the official installation instructions for your platform.

## Test Your Installation

To make sure that the installation worked, run the following Docker command. If
it produces the welcome message, you're ready to move on to the next lab.

<div class="mockup-code">
  <pre data-prefix="$"><code>npm i daisyui</code></pre>
</div>

Hello from Docker!
This message shows that your installation appears to be working correctly.

 {% include adsense.html type="multiplex" %}

To generate this message, Docker took the following steps:

1.  The Docker client contacted the Docker daemon.
2.  The Docker daemon pulled the "hello-world" image from the Docker Hub.
3.  The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
4.  The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with

 {% include adsense.html type="in-feed" %}

Share images, automate workflows, and more with a free Docker ID:
https://cloud.docker.com/ 


