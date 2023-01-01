# im7deb-docker
Creates a deb package for ImageMagick 7 in a docker container

Output of `im7deb.docker --help`:
```
im7deb-docker: build ImageMagick 7 in a docker image and create deb packages.
Resulting packages will be stored in /tmp/im7deb.
docker image and container will be removed.

Usage:
  im7deb-docker [OPTIONS]

Options:
  -h, --help              Display this help.
  --from DIST:RELEASE     Base image to build ImageMagick.
                            DIST can be one of debian or ubuntu
                            RELEASE is e.g. xenial or bullseye
                          Default: Same as host system.
  -o, --out DIR           Output directory. Default DIR: /tmp/im7deb
  --podman                Use podman instead of docker.
  -q                      ImageMagick Quantum Depth (8, 16 or 32)
                          Default: 16

Dependencies:
  docker or podman

The IMEI script to build IM7 is used by this docker script.
Thanks to: https://github.com/SoftCreatR/imei
```
