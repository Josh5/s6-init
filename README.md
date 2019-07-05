# Docker s6-init configuration for S6-Overlay

The [s6-overlay-builder project](https://github.com/just-containers/s6-overlay) is a series of init scripts and utilities to ease creating Docker images using s6 as a process supervisor.
This project provides a collection of packages containing standardised init scripts for commonly used services.


## Installation:

To use a particular init package from this project, your Dockerfile must have the following set:

* The S6 Overlay project added
* A default user **docker** added
* An ARG '**S6_INIT_PACKAGES**' naming the s6-init packages to install


### Examples:

Nginx service on a Ubuntu 16.04 image

* [Dockerfile-ubuntu](examples/Dockerfile-ubuntu)
