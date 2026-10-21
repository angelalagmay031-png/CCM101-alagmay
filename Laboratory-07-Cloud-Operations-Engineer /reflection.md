# Laboratory 07: Mission Reflection

Throughout this laboratory, I learned that monitoring a cloud environment is important for keeping applications stable, available, and efficient.

First, checking the host server's resources is necessary even when containers are running properly because containers depend on the host's CPU, memory, and disk storage. If these resources become insufficient, applications may slow down, stop responding, or crash. Checking the server's baseline helps identify potential problems before they affect users.

Second, the `docker logs` command is useful when a user reports that they cannot log into a web application. By examining the container logs, I can look for error messages, failed requests, authentication problems, or database connection issues. These details help me investigate the possible cause instead of guessing what went wrong.

Third, monitoring logs and monitoring metrics serve different purposes. Logs provide detailed records of application events, including HTTP requests and error messages. Metrics show numerical information about system performance, such as CPU utilization, memory consumption, and network activity. In this laboratory, I used `docker logs` to inspect application requests and `docker stats` to monitor the container's resource usage. Both are important for effective troubleshooting.

For large enterprise companies, monitoring thousands of containers requires centralized monitoring tools such as Prometheus and Grafana. Prometheus can collect and store performance metrics from different systems, while Grafana can display these metrics through dashboards and visualizations. These tools help operations teams identify unusual resource usage and detect potential issues across many containers.

Finally, this laboratory improved my ability to troubleshoot Linux environments by teaching me to use commands such as `free -h`, `df -h /`, `top`, `curl`, and Docker monitoring tools. I learned to verify system conditions, generate test requests, inspect logs, and evaluate container performance. Overall, I gained a better understanding of how cloud operations engineers maintain reliable services through continuous monitoring, careful investigation, and evidence-based problem-solving.
