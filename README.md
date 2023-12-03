# alpine
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FHillzacky%2Falpine.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FHillzacky%2Falpine?ref=badge_shield)

<img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/Hillzacky/alpine?style=plastic">

A minimal Docker image based on Alpine Linux with a complete package index and only 5 MB in size!

I have prepared this Dockerfile to enable SSH on the alpine docker container.
That is completely working good. 

The above Dockerfile has root enabled in the ssh server as well as run ssh on the time of docker 
container creation.
# How to build this Dockerfile.
<pre>
$ docker build -t ghcr.io/Hillzacky/alpine:master -f Dockerfile .
</pre>

# How to run the docker container with ssh ?

I have exposed the port 22 in the Dockerfile. You can use the below command to run the docker container.

<pre>
$ docker run -d -p 2222:22 ghcr.io/Hillzacky/alpine:master
</pre>

To connect the docker container via ssh.

<pre>
ssh root@localhost -p 2222
</pre>
Use Password: <b> password </b>

<img src="https://media.giphy.com/media/3o7buaZCmo40ZzIQ00/giphy.gif" width="480" height="260.9059233449477">


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FHillzacky%2Falpine.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FHillzacky%2Falpine?ref=badge_large)
