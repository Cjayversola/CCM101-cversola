# Mission 2: Build the Cloud Infrastructure Blueprint

## Mission Overview

This laboratory activity focused on investigating the basic infrastructure of a cloud server using the KillerCoda Linux environment. I examined the compute, storage, networking, and operating system resources and documented the results in my Cloud Computing portfolio.

I also researched the infrastructure services of AWS, Microsoft Azure, and Google Cloud Platform and created a simple cloud infrastructure diagram.

## Objectives

- Explain the major components of cloud infrastructure.
- Investigate hardware and software resources in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Understand how cloud infrastructure components work together.
- Create technical documentation using Markdown.
- Organize and maintain a GitHub Cloud Computing portfolio.

## Cloud Infrastructure Components

### Compute Resources

The KillerCoda server uses an Intel Xeon E312xx CPU with 1 CPU core and 1.9 GiB of RAM. These resources provide the processing power needed to run commands, applications, and services.

### Storage Resources

The main storage device is `/dev/vda1`, with a capacity of 19 GB and an ext4 filesystem. Storage provides space for the operating system, applications, configuration files, and other data.

### Networking Resources

The main network interface is `enp1s0` with the IP address `172.30.1.2/24`. A Docker bridge interface named `docker0` is also present.

### Operating System

The server runs Ubuntu 24.04.4 LTS with kernel version `6.8.0-138-generic`. The operating system manages the server resources and provides the environment for running applications and services.

## Tools Used

- KillerCoda Playground
- Ubuntu Linux
- GitHub
- Web Browser
- Draw.io / diagrams.net
- Linux command-line tools

## Linux Commands Executed

The following Linux commands were used during the investigation:

```bash
hostname
cat /etc/os-release
uname -r
lscpu
free -h
df -h
findmnt
hostname -I
ip addr show
