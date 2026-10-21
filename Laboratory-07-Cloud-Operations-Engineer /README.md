# Laboratory 07: Cloud Operations Engineer

## 1. Mission Overview

This laboratory focuses on monitoring a cloud server and managing a web application using Docker. The activities involved checking the host system's memory and disk capacity, deploying an Nginx web server, generating HTTP requests, examining application logs, and monitoring container resource consumption.

## 2. Objectives

- Determine the server's baseline RAM usage and available disk storage.
- Monitor active processes and CPU activity using Linux system tools.
- Deploy an Nginx container named `clientwebsite` using Docker.
- Simulate website visits using `curl` and generate a 404 Not Found response.
- Retrieve and analyze application logs to identify HTTP requests and errors.
- Monitor the container's CPU, memory, and network usage using `docker stats`.
- Document the results and organize screenshot evidence for the cloud operations portfolio.

## 3. Monitoring Commands Executed

| **Command** | **Purpose** |
|---|---|
| `free -h` | Displays RAM and swap memory usage. |
| `df -h /` | Checks the capacity and available storage of the root filesystem. |
| `top` | Monitors active processes and CPU activity in real time. |
| `docker run -d --name clientwebsite -p 8080:80 nginx` | Deploys the Nginx web server in a background container and maps port 8080. |
| `docker ps` | Displays currently running Docker containers. |
| `curl http://localhost:8080` | Sends HTTP requests to test the Nginx website. |
| `curl -i http://localhost:8080/hidden-admin-page` | Checks the HTTP response for a nonexistent page. |
| `docker logs clientwebsite` | Retrieves the container's application logs. |
| `docker stats` | Monitors real-time CPU, memory, and network usage. |
| `ls -l screenshots` | Verifies the screenshot files in the evidence folder. |

## 4. Skills Learned

Through this laboratory, I learned how to assess the basic health of a Linux server and monitor its resource utilization. I gained practical experience deploying a web server using Docker, testing HTTP requests with `curl`, and identifying unsuccessful requests through application logs. I also learned how to use `docker stats` to observe container performance and understand the importance of monitoring CPU, memory, and disk space. These skills helped me understand how cloud operations engineers maintain application availability, troubleshoot issues, and manage server resources efficiently.

## Repository Contents

- `README.md` — Laboratory overview, objectives, commands, and skills learned.
- `system-baseline-report.md` — Host RAM and disk storage information.
- `container-observability.md` — Application logs and real-time container metrics.
- `reflection.md` — Reflection on the laboratory experience and lessons learned.
- `screenshots/` — Evidence of host monitoring, Nginx deployment, HTTP requests, application logs, and container resource usage.
