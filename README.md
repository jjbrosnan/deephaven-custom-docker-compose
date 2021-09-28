# deephaven-custom-docker-compose

Custom docker-compose files for Deephaven-core.  These docker-compose files pull custom images built from the base Deephaven images.  They contain additional packages and functionalities.

# Contents:

Docker_Files: Custom Dockerfiles
Docker_Compose_Files: Custom docker-compose.yml files

The docker-compose files in this repository reference local custom Docker images.

# How to use these with Deephaven

To use these with Deephaven, you need to make a custom Docker image.  To do so, run the following command from the directory with the Dockerfile you would like to build with.  For example, let's say we want to use the "Super_AI" Dockerfile:

```bash
cd Docker_Files/Super_AI

docker build --tag <user>/<image_name>:<version> .
```

Check that the image exists (it should be the first on the list):

```bash
docker image ls
```

Next, go to the corresponding Docker_Compose_Files folder:

```bash
cd ../../Docker_Compose_Files/Super_AI
```

Update the image used by the grpc-api container:

```
services:
  grpc-api:
    image: <user>/<image_name>:${VERSION:-latest}
```

Lastly, start up the containers:

```bash
docker-compose up
```

Once the packages on my personal GitHub page have been tested, I will update the docker-compose.yml files to use them.
