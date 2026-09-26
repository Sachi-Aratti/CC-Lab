# Docker Lab — Experiment 1
## Containerize and Run a Simple Python Web Application

## Introduction

Docker is a containerization platform that allows applications to be packaged together with their dependencies and executed in an isolated environment called a container.

This experiment introduces the basic process of containerizing a simple Python Flask web application. The application is packaged into a Docker image and then executed as a Docker container. The running application is accessed from the host system through Docker port mapping.

The experiment also provides an understanding of the relationship between a Dockerfile, Docker image, and Docker container.

---

## Objective

The objective of this experiment is to:

- Create a simple Python Flask web application.
- Define the application environment using a Dockerfile.
- Build a Docker image from the Dockerfile.
- Create and run a container from the image.
- Map the container port to a host port.
- Access and verify the application through a web browser.
- Perform basic container lifecycle operations.

---

## Application

A simple Flask web application was created using Python.

The application contains a basic route that displays:

```text
Hello from Docker!

# `Experiment-2/README.md`

```markdown
# Docker Lab — Experiment 2
## Run, Test and Manage a Docker Container

## Introduction

This experiment focuses on running, testing, inspecting, and managing a Docker container using an existing Docker image.

The Docker image created during Experiment 1 was reused instead of building a new image. This allowed the experiment to focus on the behavior and lifecycle of a Docker container.

The experiment covered container creation, application testing, viewing logs, inspecting container configuration, accessing the container internally, stopping and restarting the container, and finally removing the container.

---

## Objective

The objective of this experiment is to:

- Reuse an existing Docker image.
- Create a new container from the image.
- Verify that the container is running.
- Test the application from the host system.
- View the container logs.
- Inspect the container configuration.
- Access the container through a shell.
- Examine files inside the container.
- Stop and restart the container.
- Verify that restarting does not create a new container.
- Remove the container while retaining the Docker image.

---

## Existing Docker Image

The image created in Experiment 1 was reused for this experiment.

The image used was:

```text
flask-docker-app
