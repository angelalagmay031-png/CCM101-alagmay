
# Container Observability

## Nginx Application Logging

### Overview

The Nginx web server was deployed as a Docker container and accessed through port 8080 to simulate user activity. Docker logs were reviewed to monitor incoming HTTP requests and identify unsuccessful requests, such as a 404 Not Found response.

### Command Used

```bash
docker logs clientwebsite
```

---

## Container Resource Monitoring

Command used: `docker stats`

| **Resource Metric** | **Observed Value** |
|---------------------|--------------------|
| Memory Consumption | 2.688 MiB |
| CPU Utilization | 0.00% |
| Memory Limit | 1.859 GiB |
| Memory Usage Percentage | 0.14% |

At the time of monitoring, the `clientwebsite` container was using approximately **2.688 MiB of memory**, equivalent to **0.14% of its 1.859 GiB memory limit**, while CPU utilization remained at **0.00%**.

---

## Importance of Application Logs

Application logs help administrators track HTTP requests and identify errors that may affect website availability. By reviewing these records, cloud engineers can investigate failed requests, determine possible causes, and resolve application issues more efficiently.
