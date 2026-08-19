# Infrastructure Report

## Linux Cloud Server Investigation

The Linux cloud server provided through the KillerCoda Playground was investigated using standard Linux commands. The following information was collected from the server environment.

| Infrastructure Information | Findings                                      |
| -------------------------- | --------------------------------------------- |
| Operating System           | Ubuntu 24.04.4 LTS (Noble Numbat)             |
| Kernel Version             | 6.8.0-136-generic                             |
| CPU Model                  | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| Number of CPU Cores        | 1                                             |
| Total RAM                  | 1.9 GiB                                       |
| Disk Capacity              | 20 GB                                         |
| Hostname                   | ubuntu                                        |
| IP Address                 | 172.30.1.2, 172.17.0.1                        |

## Operating System

The server is running Ubuntu 24.04.4 LTS, also known as Noble Numbat. Ubuntu is a Linux-based operating system commonly used for servers and cloud computing environments because of its stability, security, and extensive software support.

## Kernel Version

The Linux kernel version installed on the server is `6.8.0-136-generic`. The kernel manages important system resources such as the CPU, memory, devices, and communication between hardware and software.

## CPU

The server has an Intel Xeon E312xx processor with one available CPU core. The environment is running on a KVM virtualized platform, which shows that the server is a virtual machine running within a cloud environment.

## Memory

The server has a total of approximately 1.9 GiB of RAM. At the time of investigation, approximately 1.4 GiB was available for use.

## Storage

The main disk is a 20 GB virtual disk named `/dev/vda`. The primary partition `/dev/vda1` provides approximately 19 GB and is mounted as the root filesystem.

Additional partitions include `/dev/vda16`, which is used for `/boot`, and `/dev/vda15`, which is used for `/boot/efi`.

## Mounted File Systems

The main mounted filesystems identified during the investigation were:

* `/dev/vda1` mounted on `/` using the ext4 filesystem
* `/dev/vda16` mounted on `/boot` using the ext4 filesystem
* `/dev/vda15` mounted on `/boot/efi` using the vfat filesystem
* Several virtual filesystems such as `proc`, `sysfs`, `tmpfs`, and `devtmpfs`

These filesystems allow the operating system to organize storage and provide access to system resources and devices.

## Hostname

The hostname of the server is `ubuntu`.

## IP Address

The server reported the following IP addresses:

* `172.30.1.2`
* `172.17.0.1`

These are private IP addresses used within the virtualized cloud environment and its internal networking.

## Linux Commands Executed

The following commands were used during the investigation:

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
lsblk
df -h
findmnt
hostname
hostname -I
```

## Summary
 According to my investigation, the KillerCoda offers a virtualized Ubuntu Linux server with a 20 GB virtual disk, one CPU core, and roughly 1.9 GiB of RAM. The environment shows how the operating system, networking, memory, compute, and storage resources interact in a cloud-based Linux server.

## Evidence

The screenshot showing the Linux investigation commands and results is stored in the `screenshots` folder as `checkpoint-2.png`.
