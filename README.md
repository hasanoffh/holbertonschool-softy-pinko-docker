# Softy Pinko Docker Project

This project focuses on containerizing a full-stack web application using **Docker** and orchestrating multiple services with **Docker Compose**. It covers everything from basic container management to horizontal scaling and load balancing.

## Project Overview
The infrastructure consists of:
1.  **Proxy:** An Nginx container acting as a reverse proxy and load balancer.
2.  **Front-end:** An Nginx container serving static files.
3.  **Back-end:** A Flask-based API server processing dynamic requests.

## Learning Objectives
* How to create and manage Docker images.
* Writing efficient `Dockerfile`s.
* Orchestrating multi-container environments with `docker-compose.yml`.
* Implementing **Horizontal Scaling** using the `--scale` flag.
* Understanding Round-Robin load balancing with Nginx.

---

## Task Summary

### Task 0-4: Containerization Basics
* Building individual Dockerfiles for each service.
* Running containers independently and ensuring they communicate within a shared network.

### Task 5: Docker Compose
* Using a single `docker-compose.yml` file to spin up the entire stack (Proxy, Front-end, and Back-end) with one command:
  ```bash
  docker-compose up
