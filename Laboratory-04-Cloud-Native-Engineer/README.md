
# Laboratory 04 — The Cloud-Native Engineer

## Mission Overview

This laboratory introduced the basic concepts and workflow of cloud-native application deployment using Docker. The mission focused on understanding how containers differ from traditional Virtual Machines and applying those concepts through a practical Nginx deployment.

Using the KillerCoda Docker environment, I verified the Docker installation, downloaded an Nginx image, launched a container, exposed its web service through port mapping, tested the application locally, and managed the container through its lifecycle.

The activity demonstrates how a cloud-native approach can focus on managing application services rather than manually preparing an entire operating system for every workload.

---

## Objectives

At the completion of this laboratory, I was able to:

* Explain the main differences between Virtual Machines and containers.
* Verify Docker availability in a Linux-based cloud environment.
* Pull an application image from Docker Hub.
* Create and run a container using the Docker CLI.
* Map a host network port to a container port.
* Test a containerized web server using `curl`.
* Stop, inspect, and remove a Docker container.
* Document technical procedures using Markdown.
* Organize deployment evidence inside a GitHub portfolio.

---

## Docker Commands Executed

### Checkpoint 3 — Docker Verification

```bash
docker --version
```

```bash
docker info
```

```bash
docker version
```

### Checkpoint 4 — Nginx Deployment

```bash
docker pull nginx:latest
```

```bash
docker run -d --name cloudnova-nginx -p 8080:80 nginx:latest
```

```bash
curl http://localhost:8080
```

```bash
docker ps
```

### Checkpoint 5 — Container Lifecycle

```bash
docker ps
```

```bash
docker stop cloudnova-nginx
```

```bash
docker ps -a
```

```bash
docker rm cloudnova-nginx
```

```bash
docker ps -a
```

---

## Skills Learned

This laboratory helped me develop practical skills in container-based application deployment. I learned how Docker images are used as templates for creating containers and how the Docker CLI can control those containers from a Linux terminal.

I also practiced basic container networking through port mapping. The Nginx deployment showed how an application can become accessible from the host without manually installing the web server directly into the operating system.

Another important skill was documenting technical work in a reproducible format. Recording the commands, explanations, and screenshots in Markdown makes the deployment process easier for another administrator or developer to understand and repeat.

---

## Challenges Encountered

One challenge during the activity was understanding the difference between an image and a container. The Nginx image acts as the packaged source used to create a container, while the container represents the running instance of that image.

Another challenge was understanding port mapping. The web server listens on port 80 inside the container, but I accessed it through port 8080 on the Docker host. The `-p 8080:80` option connected these two ports.

The container lifecycle also reinforced the difference between stopping and removing a container. A stopped container still exists and can be listed with `docker ps -a`, while `docker rm` removes that container from the Docker environment.

---

## Evidence

Screenshots for this laboratory are located in the `screenshots` directory.

| Screenshot                | Evidence                                         |
| ------------------------- | ------------------------------------------------ |
| `docker-version.png`      | Docker installation and environment verification |
| `nginx-running.png`       | Successful Nginx HTTP response                   |
| `container-lifecycle.png` | Container stop, verification, and removal        |

---

## Portfolio Progress

Laboratory 04 expands my cloud computing portfolio from cloud fundamentals and infrastructure planning into practical cloud-native operations. The activity demonstrates a transition from understanding cloud concepts to interacting directly with a container runtime and deploying an actual service.
