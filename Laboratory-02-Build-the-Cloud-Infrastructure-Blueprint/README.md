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
```

These commands were used to identify the server's operating system, kernel, CPU, memory, storage, mounted filesystems, hostname, and network configuration.

## Skills Learned

During this laboratory activity, I learned how to inspect a Linux cloud environment using command-line tools. I also learned how compute, storage, networking, and operating systems work together in cloud infrastructure.

I improved my Markdown documentation skills and learned how to organize technical evidence and project files in GitHub. I also gained experience comparing infrastructure services from different cloud providers and creating a basic cloud architecture diagram.

## Challenges Encountered

One challenge was understanding the different Linux commands and interpreting their output. I also had to organize the screenshots and documentation correctly inside the GitHub laboratory folder.

Another challenge was understanding the equivalent infrastructure services offered by AWS, Microsoft Azure, and Google Cloud. Researching their official documentation helped me understand how different providers offer similar cloud infrastructure capabilities under different service names.
