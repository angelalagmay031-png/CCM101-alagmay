# Infrastructure Report

## Checkpoint 2 – Investigate the Cloud Server

The Linux cloud server was investigated using the KillerCoda terminal.
The following information was collected from the server.

### 1. Operating System

- **Operating System:** Ubuntu 24.04.4 LTS
- **Release:** Ubuntu 24.04
- **Codename:** Noble

### 2. Kernel Version

- **Kernel Version:** 6.8.0-138-generic

### 3. CPU Model

- **CPU Model:** Intel Xeon E312xx (Sandy Bridge, IBRS update)

### 4. Number of CPU Cores

- **CPU Cores:** 1

### 5. Total RAM

- **Total RAM:** 1.9 GiB
- **Used RAM:** 414 MiB
- **Free RAM:** 867 MiB
- **Available RAM:** 1.5 GiB
- **Swap:** 1.0 GiB

### 6. Disk Capacity

- **Main Disk:** /dev/vda1
- **Capacity:** 19 GB
- **Used:** 5.4 GB
- **Available:** 13 GB
- **Usage:** 30%
- **Mounted on:** /

Additional partitions:
- **/dev/vda16:** 881 MB, mounted on /boot
- **/dev/vda15:** 105 MB, mounted on /boot/efi

### 7. Mounted File Systems

The following file systems were identified:

- `/` – /dev/vda1 – ext4
- `/boot` – /dev/vda16 – ext4
- `/boot/efi` – /dev/vda15 – vfat
- `/sys` – sysfs
- `/proc` – proc
- `/dev` – devtmpfs
- `/dev/shm` – tmpfs
- `/run` – tmpfs
- `/sys/fs/cgroup` – cgroup2
- `/sys/fs/bpf` – bpf
- `/sys/kernel/debug` – debugfs
- `/sys/kernel/tracing` – tracefs
- `/sys/kernel/config` – configfs
- `/dev/pts` – devpts
- `/dev/mqueue` – mqueue

### 8. Hostname

- **Hostname:** ubuntu

### 9. IP Address

- **Primary IP Address:** 172.30.1.2
- **Docker Network IP:** 172.17.0.1
- **Loopback:** 127.0.0.1

## Summary

The cloud server is running Ubuntu 24.04.4 LTS with a
6.8.0-138-generic kernel. It has an Intel Xeon E312xx CPU
with 1 CPU core and 1.9 GiB of RAM. The main disk has a
capacity of 19 GB, with approximately 13 GB available.
The hostname of the server is `ubuntu`, and its primary
network IP address is `172.30.1.2`.

The investigation was completed using Linux commands in the
KillerCoda terminal, and the results were documented for
Checkpoint 2.
