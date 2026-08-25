# Cloud Infrastructure Components

## 1. Compute Resources

### Purpose

Compute resources are responsible for carrying out the instructions given by users and applications. The processor and memory work together to execute commands, run programs, and handle active processes.

### Importance in Cloud Computing

Computing power is one of the main requirements of a cloud environment because applications and services need resources to operate. Cloud systems can allocate more or fewer resources depending on the amount of work being performed.

### KillerCoda Linux Environment

In KillerCoda, the Linux server is provided with virtual processing and memory resources. These resources are used whenever commands are executed or programs are running. The `lscpu` command was used to view CPU information, while `free -h` was used to check the available memory.

---

## 2. Storage Resources

### Purpose

Storage resources provide a location where system files, programs, configurations, and personal or laboratory data can be saved.

### Importance in Cloud Computing

Cloud storage allows information to be retained and accessed when needed. It is important for applications because data must have a dependable storage location. Cloud environments can also provide different storage capacities based on the requirements of a workload.

### KillerCoda Linux Environment

The KillerCoda server has disk space used by Ubuntu, system files, installed packages, and files created during the laboratory activities. The `df -h` command was used to check the disk usage and available storage in the Linux environment.

---

## 3. Networking Resources

### Purpose

Networking resources provide the connection needed for devices and systems to exchange information. Network interfaces and IP addresses help establish communication between the Linux server and other systems.

### Importance in Cloud Computing

Networking makes it possible for users to access cloud resources remotely. It also allows different cloud services, servers, and applications to communicate and transfer information.

### KillerCoda Linux Environment

The KillerCoda server uses a virtual network connection to communicate with external systems and cloud services. Network interfaces and IP address information can be examined using the `ip addr` command. The `hostname -I` command can also be used to display the server's IP address.

---

## 4. Operating System

### Purpose

The operating system serves as the main software layer that controls system resources and provides users with tools for managing files, processes, applications, and hardware-related resources.

### Importance in Cloud Computing

Cloud servers depend on an operating system to manage the resources assigned to them. It provides the environment needed for applications and services to operate while also handling users, processes, storage, and network connections.

### KillerCoda Linux Environment

The operating system used in the KillerCoda environment is **Ubuntu 24.04 LTS**. It provides a command-line environment where Linux commands can be executed to inspect and manage the server. The `lsb_release -a` command was used to identify the Ubuntu version, while `uname -r` was used to check the Linux kernel version.

---

## Relationship Between the Components

These infrastructure components depend on one another to create a functional cloud environment. The operating system coordinates the available CPU and memory, manages access to storage, and handles network communication. Compute resources execute workloads, storage keeps the required data, and networking connects the environment to other systems. Together, they form the basic infrastructure needed for running applications and services in the KillerCoda Linux environment.
