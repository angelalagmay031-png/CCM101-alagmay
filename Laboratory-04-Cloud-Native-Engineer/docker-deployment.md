
# Docker Deployment and Container Lifecycle

## Environment Verification

Before deploying the web server, I verified that Docker was available in the KillerCoda environment.

### Check Docker Version

```bash
docker --version
```

This command displays the installed Docker CLI version and confirms that the Docker command is available.

### Check Docker Environment

```bash
docker info
```

This command displays information about the Docker engine, including the server configuration and available resources.

---

## Nginx Deployment

### Pull the Nginx Image

```bash
docker pull nginx:latest
```

This command downloads the latest Nginx image from Docker Hub so that it can be used to create a container.

### Start the Nginx Container

```bash
docker run -d --name cloudnova-nginx -p 8080:80 nginx:latest
```

This command creates and starts a detached Nginx container named `cloudnova-nginx` while mapping host port 8080 to port 80 inside the container.

### Test the Web Server

```bash
curl http://localhost:8080
```

This command sends a local HTTP request to the mapped port and verifies that the Nginx web server is responding.

---

## Container Lifecycle Operations

### 1. List Running Containers

```bash
docker ps
```

This command displays all currently running Docker containers and their runtime information.

### 2. Stop the Container

```bash
docker stop cloudnova-nginx
```

This command stops the running Nginx container while keeping the container itself available for later management.

### 3. Verify the Container State

```bash
docker ps -a
```

This command lists both active and stopped containers, allowing the stopped Nginx container to be confirmed.

### 4. Remove the Container

```bash
docker rm cloudnova-nginx
```

This command removes the stopped Nginx container from the Docker host.

### 5. Confirm Removal

```bash
docker ps -a
```

This final check confirms that `cloudnova-nginx` has been removed from the list of containers.

---

## Port Mapping

The deployment used the following mapping:

```text
8080:80
```

Port `8080` is the port exposed on the Docker host, while port `80` is the port used by Nginx inside the container. This mapping allows requests sent to `localhost:8080` on the host to reach the Nginx service running inside the container.

## Evidence

The terminal screenshots for this mission are stored in the `screenshots` directory:

* `docker-version.png` — Docker environment verification
* `nginx-running.png` — Successful Nginx HTTP response
* `container-lifecycle.png` — Container management operations
