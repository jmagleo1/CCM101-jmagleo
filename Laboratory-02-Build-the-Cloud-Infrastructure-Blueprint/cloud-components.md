**Cloud Infrastructure Components**
**Introduction**

Cloud infrastructure is made up of different resources that work together to provide computing services. In the KillerCoda Linux environment, examples of compute, storage, networking, and operating system resources can be observed directly from the server.

1. ** Compute Resources**
   Example: Intel Xeon E312xx CPU with 1 CPU core.
   
   Purpose:
The processing power required to execute commands, applications, services, and other workloads is provided by compute resources.

Importance in cloud computing
Organizations can run applications without maintaining physical servers thanks to compute resources. Depending on the demands of the workload, cloud providers can assign or modify computer resources.

Relation to the KillerCoda Environment:
One CPU core is provided by the KillerCoda server via a virtualized environment. The processor and CPU configuration were determined using the lscpu command.
2. **Storage Resources**

Example: 20 GB virtual disk /dev/vda.

Purpose:
Storage resources are used to save the operating system, applications, configuration files, and user data.

Importance in Cloud Computing:
Cloud storage provides a way to store data reliably and access it when needed. It also allows organizations to manage storage without directly maintaining physical storage hardware.

Relation to the KillerCoda Environment:
The Linux server has a 20 GB virtual disk. The main partition /dev/vda1 is mounted on / and uses the ext4 filesystem. The lsblk and df -h commands were used to investigate the storage resources.

3. **Networking Resources**

Examples: IP addresses 172.30.1.2 and 172.17.0.1.

Purpose:
Networking resources allow computers, servers, applications, and users to communicate with one another.

Importance in Cloud Computing:
Networking enables cloud servers to communicate with other services and systems. It is essential for accessing applications, transferring data, and connecting cloud resources.

Relation to the KillerCoda Environment:
The server has private IP addresses assigned within its virtualized environment. The hostname -I command was used to identify the IP addresses of the Linux server.

4. **Operating System**

Example: Ubuntu 24.04.4 LTS (Noble Numbat).

Purpose:
The operating system manages the server's hardware and software resources and provides an environment where applications and commands can run.

Importance in Cloud Computing:
Operating systems provide the foundation for cloud workloads. They allow cloud servers to run applications, manage resources, provide security controls, and support system administration.

Relation to the KillerCoda Environment:
The KillerCoda server runs Ubuntu 24.04.4 LTS with Linux kernel version 6.8.0-136-generic. The operating system information was identified using the cat /etc/os-release command.

**Relationship Between the Components**
Together, the infrastructure elements create a working cloud server. Processing power is provided by the CPU, memory allows processes to run, storage stores system and application data, networking facilitates communication, and these resources are managed by the operating system.
These elements are integrated into a virtualized Linux server in the KillerCoda environment. This illustrates how cloud infrastructure resources collaborate.
to offer computer services.

**Conclusion**

The main elements of cloud infrastructure were found through the examination of the KillerCoda environment. Planning, implementing, and maintaining cloud-based systems require an understanding of compute, storage, networking, and operating system resources.
