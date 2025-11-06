# version-1

This is a simple Node.js application.

## Prerequisites

- Docker
- Node.js

## Build the Docker image

To build the Docker image, run the following command:

```bash
docker build -t version-1 .
```

## Run the Docker container

To run the Docker container, use the following command:

```bash
docker run -p 3000:3000 version-1
```

## Using Docker Compose

To build and run the services defined in the `docker-compose.yml` file, use the following command:

```bash
docker-compose up
```

To run the services in detached mode, use the `-d` flag:

```bash
docker-compose up -d
```

To stop the services, use the following command:

```bash
docker-compose down
```

## Push the Docker image to a registry

To push the Docker image to a container registry like Docker Hub, follow these steps:

1.  **Log in to your Docker registry:**

    ```bash
    docker login
    ```


2.  **Tag the image:**

    Replace `your-dockerhub-username` with your Docker Hub username.

    ```bash
    docker tag version-1 your-dockerhub-username/version-1:latest
    ```

3.  **Push the image:**

    ```bash
    docker push your-dockerhub-username/version-1:latest
    ```
