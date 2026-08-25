# Infrastructure Report

## Server Information

The Linux server used in this laboratory activity is running on the KillerCoda Playground.

| Information | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Kernel Version | 6.8.0-138-generic |
| CPU Model | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| CPU Cores | 1 |
| Total RAM | 1.9 GiB |
| Hostname | ubuntu |
| IP Address | 172.30.1.2 |

## Storage Information

The main filesystem is `/dev/vda1`, which uses the ext4 filesystem and has a total capacity of 19 GB. The system also contains mounted filesystems for `/boot` and `/boot/efi`.

| Filesystem | Size | Mounted On | Filesystem Type |
|---|---:|---|---|
| /dev/vda1 | 19G | / | ext4 |
| /dev/vda16 | 881M | /boot | ext4 |
| /dev/vda15 | 105M | /boot/efi | vfat |

The main storage device has approximately 5.4 GB of used space and 13 GB of available space.

## Network Information

The server hostname is `ubuntu`. The primary network interface is `enp1s0` with the IP address `172.30.1.2/24`.

A Docker bridge interface named `docker0` is also present with the address `172.17.0.1/16`.

## Mounted File Systems

The `findmnt` command showed several mounted filesystems. The main root filesystem is mounted at `/` from `/dev/vda1`. Other important mounted locations include `/boot` and `/boot/efi`.

## Linux Commands Used

The following commands were used to investigate the server:

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

## Summary

The KillerCoda environment provides a basic Linux cloud server with Ubuntu 24.04.4 LTS, one CPU core, 1.9 GiB of RAM, and a 19 GB main storage device. The server also has an active network interface with a private IP address. These resources demonstrate the basic compute, storage, networking, and operating system components commonly found in cloud infrastructure.
