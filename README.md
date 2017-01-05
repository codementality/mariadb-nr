# MariaDB (non-root)
An implementation of dockerized MariaDB running as non-root user mysql

## Use
This image is modeled after the official MariaDB version 10.1.20.  The user instructions for this container are the same as those for the official container, which can be seen on Docker Hub here:  https://hub.docker.com/_/mariadb/

The documentation for use of this image can be found here:  https://github.com/docker-library/docs/tree/master/mariadb

## Differences from the Official MariadDB image
This image has a few significant differences:

* It runs as the mysql user by default (the official container runs as root)
* It removes several unnecessary user accounts

This image should be a drop-in replacement for mariadb:10.1.20, but compliant with _CIS Docker 1.12.0 Benchmark_ recommendation 4.1 **Create a user for the container**.

## Work In Progress
It is a work in progress, and very well may have additional modifications in the future to comply with _CIS Docker 1.12.0 Benchmark_ recommendation 4.3 **Do not install unnecessary packages in the container**.  This README will be updated when this occurs.

At this time this image is based on the official debian:jessie image.

## Docker Hub
https://hub.docker.com/r/codementality/mariadb-nr/
