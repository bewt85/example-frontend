example-frontend
================

This is part of [mayfly](https://github.com/bewt85/mayfly) which demonstrates the 
concept of testing groups of versions of services in short lived virtual environments.

This is a docker container which runs a simple frontend service.  It comes in (at least)
two versions:

- release/0.0.1; and
- release/0.0.2

Note that, as with other [mayfly](https://github.com/bewt85/mayfly) services, it passes on
the `x-mayfly` header in requests to other services (if present).

You can build your own versions of the containers by setting the following environment variable 
to your docker index username (if you don't it uses mine) and running this bash script:

```
export DOCKER_ACCOUNT_NAME=<your_name>
sudo -E ./build.sh
```
