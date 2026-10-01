# Basic Dockerfile

A simple Docker project created to practice the fundamentals of building and running Docker images.

This project is based on the **Basic Dockerfile** project from roadmap.sh.

## Objective

The goal of this project is to create a Docker image based on Alpine Linux that prints a message to the console when a container is started.

## Technologies

- Docker
- Alpine Linux

## Project Structure

```text
.
├── Dockerfile
└── README.md
```

## Dockerfile

The Dockerfile uses the latest Alpine Linux image as its base image and defines a command that prints:

```text
Hello, Captain!
```

when the container starts.

## Build the Image

From the project directory, build the Docker image:

```bash
docker build -t devops01 .
```

### Command explanation

- `docker build` — builds a Docker image from a Dockerfile.
- `-t devops01` — assigns the name/tag `devops01` to the image.
- `.` — uses the current directory as the Docker build context.

## Run the Container

Run a container from the image:

```bash
docker run devops01
```

Expected output:

```text
Hello, Captain!
```

The container exits immediately after printing the message because the `echo` command has finished executing.

## What I Learned

Through this project I practiced:

- Creating a basic Dockerfile
- Using a lightweight Linux base image
- Understanding the difference between a Docker image and a container
- Building Docker images with `docker build`
- Running containers with `docker run`
- Understanding the purpose of `CMD`
- Understanding Docker build context

## Roadmap.sh Project

This project was completed as part of the roadmap.sh DevOps projects:

**Basic Dockerfile**

Project page:

https://roadmap.sh/projects/basic-dockerfile
