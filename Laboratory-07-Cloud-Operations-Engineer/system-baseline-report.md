# System Baseline Report

## Host System Baseline

The Linux server was checked before deploying the web application to determine its current resource condition.

| Resource              | Result                             |
| --------------------- | ---------------------------------- |
| Total RAM             | 1903.2 MiB (approximately 1.9 GiB) |
| RAM Used              | 462.0 MiB                          |
| RAM Available         | 1441.2 MiB                         |
| Root Storage Capacity | 19 GB                              |
| Storage Used          | 5.4 GB                             |
| Storage Available     | 13 GB                              |
| CPU Usage             | 0.3%                               |
| CPU Idle              | 99.7%                              |
| Load Average          | 0.00, 0.02, 0.03                   |
| Total Processes       | 127                                |

## Disk Space Importance

Checking disk space is important before a massive traffic surge because the server needs enough available storage for application files, logs, temporary data, and other system activities.

## Evidence

* `memory-check.png` – RAM usage output
* `disk-check.png` – Root disk storage output
* `top` – CPU load and active processes
