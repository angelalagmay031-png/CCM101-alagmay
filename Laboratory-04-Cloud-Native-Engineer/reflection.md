
# Mission 4 Reflection

This laboratory gave me a more practical understanding of why containers are widely used in cloud-native environments. One of the biggest differences I noticed between a Docker container and a Virtual Machine is the setup process. A VM normally needs a complete operating system to be created and started before the application can run. A Docker container, on the other hand, can start directly from an existing image without requiring another full operating system. In this activity, the Nginx service could be deployed with only a few commands, which made the process much more lightweight and repeatable.

The `-p 8080:80` option was also important because the Nginx service was listening on port 80 inside the container. The host computer was not automatically using that internal container port. Port mapping connected host port 8080 to container port 80, allowing me to access the web server through `http://localhost:8080`. Without this mapping, the service would not be directly accessible through that host port.

I also learned that `docker rm` removes the container itself. Any data stored only inside the container's writable layer should not be treated as permanent storage. This showed me why persistent application data should normally be placed in appropriate Docker volumes or external storage instead of relying on the container's temporary filesystem.

Containerization can also change how developers and IT operations teams collaborate. Developers can package an application and its dependencies into a consistent image, while operations teams can deploy and manage that same image across environments. This supports a more consistent DevOps workflow because deployment becomes more standardized and reproducible.

Finally, my GitHub portfolio is evolving from a collection of individual laboratory activities into a record of practical cloud skills. This laboratory added Docker, container lifecycle management, networking, and technical documentation to the concepts I have already studied.
