# System Baseline Report

## 1. Overview

This report documents the initial health check of the Ubuntu host used for Laboratory Activity 7. The purpose is to examine the server's memory, disk capacity, and CPU activity before deploying the client website.

## 2. Memory Assessment

Based on the output of the `free -h` command:

* **Total RAM:** 1.9 GiB
* **Used Memory:** 409 MiB
* **Free Memory:** 1.1 GiB
* **Available Memory:** 1.5 GiB
* **Swap Space:** 1.0 GiB
* **Used Swap:** 0 B

The server has 1.9 GiB of total RAM, with 1.5 GiB available for applications and other processes. This indicates that sufficient memory was available at the time of the check.

## 3. Disk Assessment

Based on the output of the `df -h /` command:

* **Root Filesystem:** `/`
* **Total Storage Capacity:** 19 GiB
* **Used Storage:** 5.5 GiB
* **Available Storage:** 13 GiB
* **Storage Usage:** 30%

The root filesystem has 13 GiB of available storage, with 30% of its capacity currently used. Checking disk space before a major traffic surge is important because insufficient storage can prevent the server from writing logs, temporary files, and application data, which may affect service availability.

## 4. CPU and Process Monitoring

The `top` command is used to observe running processes, CPU activity, and system load. These details help identify potential resource issues before and during application deployment.

## 5. Evidence

* `screenshots/memory-check.png` — Evidence of the host's RAM usage and availability.
* `screenshots/disk-check.png` — Evidence of the root filesystem's storage capacity and usage.

## 6. Conclusion

The host baseline shows that the server has 1.9 GiB of RAM and 19 GiB of total root filesystem storage. At the time of measurement, 1.5 GiB of memory and 13 GiB of disk space were available. These results provide a starting point for monitoring the server's health and comparing host resources with the Nginx container's performance during the remaining activity.
