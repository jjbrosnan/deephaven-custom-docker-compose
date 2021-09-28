# deephaven-custom-docker-compose

Custom docker-compose and Dockerfile files for Deephaven-core.  The docker-compose files pull custom images built from the base Deephaven images.  The Dockerfiles contain the rules to build the custom images.  They contain additional packages and functionalities on top of Deephaven-core's base `grpc-api` image.

# Contents:

Docker_Files: Custom Dockerfiles
Docker_Compose_Files: Custom docker-compose.yml files

The docker-compose files in this repository reference local custom Docker images.

# How to use these with Deephaven

In one of the Docker_Compose_Files directories (for example, Super_AI), run:

```bash
docker-compose up
```

The necessary images will be created and then you can run Deephaven!
