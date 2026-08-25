# Cloud Infrastructure Components

## 1. Compute Resources

The Linux server provided by KillerCoda has an Intel Xeon E312xx CPU with 1 CPU core and 1.9 GiB of RAM. These resources are used to process commands, run applications, and perform computing tasks.

Compute resources are important in cloud computing because applications need processing power and memory to operate. In the KillerCoda environment, the CPU and RAM allow the Ubuntu server to execute Linux commands and run services.

## 2. Storage Resources

The main storage device found in the server is `/dev/vda1`, which has a capacity of 19 GB. It uses the ext4 filesystem and is mounted at `/`.

Storage is important because cloud systems need space for the operating system, applications, configuration files, and user data. In the KillerCoda environment, the storage is used by Ubuntu and the files and services running on the server.

## 3. Networking Resources

The main network interface is `enp1s0`, which has the IP address `172.30.1.2/24`. The system also has a Docker bridge interface called `docker0` with the address `172.17.0.1/16`.

Networking is important in cloud computing because it allows servers, users, applications, and cloud services to communicate with each other. In the KillerCoda environment, the network interface provides connectivity for the Linux server.

## 4. Operating System

The server is running Ubuntu 24.04.4 LTS with kernel version `6.8.0-138-generic`.

The operating system manages the server's hardware and software resources. It is important in cloud computing because it provides the environment where applications, services, and management tools can run. In KillerCoda, Ubuntu provides the command-line environment used to investigate and manage the cloud server.
