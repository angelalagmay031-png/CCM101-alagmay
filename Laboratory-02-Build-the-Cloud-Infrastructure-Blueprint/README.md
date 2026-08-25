
# Cloud Infrastructure Mission

## 1. Mission Overview

This laboratory mission introduced me to the basic process of investigating a cloud-based Linux server. Using the KillerCoda environment, I explored the server through the terminal and collected information about its operating system, hardware, storage, file systems, and network configuration.

Instead of relying on a graphical interface, I used Linux commands to discover how the server was configured. The results were then organized and documented in Markdown for future reference.

## 2. Objectives

The mission was designed to help me:

* Explore a real Linux cloud environment.
* Identify the server's operating system and kernel.
* Examine CPU, memory, and storage resources.
* Understand mounted file systems.
* Identify the hostname and network addresses.
* Practice using Linux command-line tools.
* Develop proper technical documentation habits.
* Record and organize infrastructure findings clearly.

## 3. Cloud Infrastructure Components

The cloud server investigated during the mission contained the following components:

| Component            | Information                                   |
| -------------------- | --------------------------------------------- |
| **Operating System** | Ubuntu 24.04.4 LTS                            |
| **Kernel**           | 6.8.0-138-generic                             |
| **CPU**              | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| **CPU Cores**        | 1                                             |
| **RAM**              | 1.9 GiB                                       |
| **Main Storage**     | 19 GB                                         |
| **Hostname**         | `ubuntu`                                      |
| **Primary IP**       | `172.30.1.2`                                  |
| **Docker Network**   | `172.17.0.1`                                  |

These components work together to provide the computing environment where applications, services, networking, and system processes can operate.

## 4. Tools Used

The following tools and technologies were used:

* **KillerCoda** – Provided the cloud-based Linux environment.
* **Linux Terminal** – Used to investigate and collect server information.
* **GitHub** – Used to organize and store laboratory files.
* **Markdown** – Used to create readable technical documentation.

## 5. Linux Commands Executed

| Command          | What I Used It For                               |
| ---------------- | ------------------------------------------------ |
| `lsb_release -a` | Identified the Linux distribution and version.   |
| `uname -r`       | Checked the current kernel version.              |
| `lscpu`          | Examined processor information.                  |
| `nproc`          | Determined the number of CPU cores.              |
| `free -h`        | Checked memory usage and available RAM.          |
| `df -h`          | Investigated disk capacity and usage.            |
| `findmnt`        | Viewed mounted file systems.                     |
| `hostname`       | Identified the server name.                      |
| `hostname -I`    | Displayed assigned IP addresses.                 |
| `ip addr`        | Examined network interfaces and their addresses. |

## 6. Skills Learned

This mission helped me develop practical skills that I can use in future IT and cloud-related activities. I learned how to navigate a Linux server through the command line and how to interpret information returned by different commands.

I also learned how to identify system resources such as CPU, RAM, storage, and network interfaces. Another important skill I developed was documenting technical information in an organized way using Markdown. I became more comfortable reading terminal output and identifying which information is important for an infrastructure report.

## 7. Challenges Encountered

One challenge I experienced was dealing with the amount of information displayed by commands such as `findmnt` and `ip addr`. At first, the output looked confusing because there were many file systems, interfaces, and technical details.

I also had to understand the difference between the server's primary IP address and the Docker network address. After examining the network interfaces, I identified `172.30.1.2` as the main server IP and `172.17.0.1` as the Docker network address.

Another challenge was making sure that the information I documented matched the actual server output. This taught me that technical documentation should be based on verified information rather than assumptions.

## 8. Key Takeaway

The most important lesson I gained from this mission is that **understanding a cloud server starts with knowing what is running inside it**. By using simple Linux commands, I was able to investigate the server's resources and configuration without depending on a graphical interface.

This activity gave me a stronger foundation in Linux, cloud infrastructure, networking, and technical documentation.
