# Docker Image
The docker image is based on the confluent docker image and adds only a start script and a readiness check script.
## Makefile 
The [makefile](Makefile) contained in the docker directory has three commands.
- The `build` command will build the Docker image locally.
- The `push` command will push the image, provided you have correct permissions, 
to grc.io/containers repository.
- The `all` command will perform the `build` command.
