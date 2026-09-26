# Docker Lab — Experiments 1 & 2

This repository contains the implementation, documentation, and screenshot evidence for **Docker Lab Experiments 1 and 2**.

The experiments introduce the fundamentals of Docker by starting with a simple Python Flask web application, containerizing the application, running it using Docker, and then learning how to manage the resulting Docker containers through their complete lifecycle.

---

# Table of Contents

- [Introduction](#introduction)
- [Environment and Tools](#environment-and-tools)
- [Experiment 1 — Containerize and Run a Simple Python Web Application](#experiment-1--containerize-and-run-a-simple-python-web-application)
  - [Objective](#objective)
  - [Concept](#concept)
  - [Application Structure](#application-structure)
  - [Step 1 — Verify Docker Installation](#step-1--verify-docker-installation)
  - [Step 2 — Test Docker](#step-2--test-docker)
  - [Step 3 — Create the Flask Application](#step-3--create-the-flask-application)
  - [Step 4 — Create requirements.txt](#step-4--create-requirementstxt)
  - [Step 5 — Create the Dockerfile](#step-5--create-the-dockerfile)
  - [Step 6 — Build the Docker Image](#step-6--build-the-docker-image)
  - [Step 7 — Verify the Docker Image](#step-7--verify-the-docker-image)
  - [Step 8 — Create and Run the Container](#step-8--create-and-run-the-container)
  - [Step 9 — Verify the Running Container](#step-9--verify-the-running-container)
  - [Step 10 — Access the Application](#step-10--access-the-application)
  - [Step 11 — Container Lifecycle](#step-11--container-lifecycle)
  - [Experiment 1 Result](#experiment-1-result)
- [Experiment 2 — Run, Test and Manage a Docker Container](#experiment-2--run-test-and-manage-a-docker-container)
  - [Objective](#objective-1)
  - [Concept](#concept-1)
  - [Step 1 — Verify the Existing Image](#step-1--verify-the-existing-image)
  - [Step 2 — Create a New Container](#step-2--create-a-new-container)
  - [Step 3 — Check Container Status](#step-3--check-container-status)
  - [Step 4 — Test the Application](#step-4--test-the-application)
  - [Step 5 — View Container Logs](#step-5--view-container-logs)
  - [Step 6 — Inspect the Container](#step-6--inspect-the-container)
  - [Step 7 — Enter the Container](#step-7--enter-the-container)
  - [Step 8 — Check Files Inside the Container](#step-8--check-files-inside-the-container)
  - [Step 9 — Check the Working Directory](#step-9--check-the-working-directory)
  - [Step 10 — Exit the Container](#step-10--exit-the-container)
  - [Step 11 — Stop the Container](#step-11--stop-the-container)
  - [Step 12 — Start the Container Again](#step-12--start-the-container-again)
  - [Step 13 — Verify the Same Container](#step-13--verify-the-same-container)
  - [Step 14 — Remove the Container](#step-14--remove-the-container)
  - [Step 15 — Verify the Docker Image](#step-15--verify-the-docker-image)
  - [Experiment 2 Result](#experiment-2-result)
- [Docker Image vs Docker Container](#docker-image-vs-docker-container)
- [Port Mapping](#port-mapping)
- [Docker Commands Used](#docker-commands-used)
- [Repository Structure](#repository-structure)
- [Conclusion](#conclusion)

---

# Introduction

Docker is a platform used to package and run applications in isolated environments called **containers**.

A Docker container contains the application and the dependencies required to run it. This allows an application to behave consistently across different environments without requiring all dependencies to be installed directly on the host machine.

In these experiments, a simple Python Flask web application is used to understand the basic Docker workflow.

The overall process covered in the two experiments is:

```text
Python Flask Application
          |
          v
     Dockerfile
          |
          v
     Docker Image
          |
          v
    Docker Container
          |
          v
      Port Mapping
          |
          v
     Web Application