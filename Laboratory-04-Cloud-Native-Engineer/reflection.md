# Mission 4 Reflection

## 1. How does the boot time and setup process of a Docker container compare to installing an operating system on a Virtual Machine?

A Docker container can be started much faster than a Virtual Machine because it does not need to boot a complete guest operating system. In this laboratory, the Nginx application was deployed using a Docker image and a single `docker run` command. A VM generally requires the operating system to be installed, configured, and booted before the application can be installed and used. This makes containers convenient for applications that need to be deployed quickly and consistently.

## 2. Why is port mapping (`-p 8080:80`) necessary when running a web server inside a container?

Port mapping connects a port on the Docker host to a port inside the container. In this activity, Nginx listens on port 80 inside the container, while I accessed the service through port 8080 on the host. The `-p 8080:80` option allows requests sent to `localhost:8080` to reach the Nginx service on port 80 inside the container. Without the mapping, the Nginx service would not be directly accessible through the host's port 8080.

## 3. What happens to the data inside a container when you use the `docker rm` command?

The `docker rm` command removes the specified container from the Docker environment. Data stored only in the container's writable layer is removed along with the container and should not be considered permanent storage. This is why applications that need persistent data should use Docker volumes or another external storage solution. In this activity, removing `cloudnova-nginx` deleted the container after it had been stopped.

## 4. How do you think containerization changes the way software developers and IT operations teams work together (DevOps)?

Containerization can make collaboration between developers and IT operations teams more consistent because an application and its dependencies can be packaged into the same container image. Developers can test the application in an environment that can closely match the deployment environment. Operations teams can then use the same image when deploying the application. This reduces differences between development and deployment environments and supports a more standardized DevOps workflow.

## 5. How is your GitHub portfolio evolving?

My GitHub portfolio is gradually becoming a record of the practical cloud computing skills I have developed throughout the laboratory activities. In this laboratory, I added containerization, Docker commands, application deployment, port mapping, container lifecycle management, and technical documentation to my previous cloud computing work. I also learned the importance of keeping screenshots and Markdown documentation organized so that my work can be reviewed and reproduced. As I complete more laboratories, the repository can serve as evidence of my progress from basic cloud concepts toward more practical cloud-native technologies.
