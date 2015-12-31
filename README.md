# docker-apt-cacher-ng
apt-cacher-ng service dockerized

Example from https://docs.docker.com/engine/examples/apt-cacher-ng/

## Getting started

Build:
> docker build -t apt-cacher .

Run:
> docker run -d -p 3142:3142 --name apt-cacher-run joaquindlz/docker-apt-cacher-ng

... and then you can run containers with:
> docker run -t -i --rm --link apt-cacher-run:apt-cache -e "http_proxy=http://apt-cache:3142/" debian bash

## Links

Docker hub: https://hub.docker.com/r/joaquindlz/docker-apt-cacher-ng/

Github: https://github.com/joaquindlz/docker-apt-cacher-ng/
