[![Build Status](https://travis-ci.org/kennethlimcp/armhf-ghost.svg?branch=master)](https://travis-ci.org/kennethlimcp/armhf-ghost)

### Automated build for Ghost armhf image

This repo contains a modified [Dockerfile](Dockerfile) that works for armhf and a base image that contains **qemu** to modify the runtime environment, allowing armhf images to be built using x86 machines.


Original repo: https://github.com/docker-library/ghost

The automated build can be viewed/pulled at: https://hub.docker.com/r/kennethlimcp/armhf-ghost/

### Steps to update [GHOST](https://ghost.org) version

```sh
$ git checkout master
$ ./update.sh
$ git add Dockerfile
$ git commit
$ git tag x.x.x
$ git push origin <tag_name>
$ git push
```
