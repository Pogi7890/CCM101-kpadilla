# Cloud Infrastructure Components

## Compute

Compute refers to the processing resources used to run applications and services. CPU cores perform instructions, while memory supports running programs and processes.

### Importance

Compute resources are necessary because applications need processing power to perform tasks. Cloud platforms allow computing resources to be adjusted according to the needs of a workload.

### Observed Example

The investigated environment contains one CPU core and approximately 1.9 GiB of RAM.

---

## Storage

Storage is used to maintain system files, applications, configurations, and user data.

### Importance

Data must remain available even after an application or process stops. Storage provides a location where important files can be saved and retrieved when needed.

### Observed Example

The main storage device is /dev/vda1, which uses the ext4 filesystem and has a total capacity of 19 GB.

---

## Networking

Networking enables cloud resources, applications, and users to communicate with one another.

### Importance

Without network connectivity, users would not be able to access cloud services. Networking also allows infrastructure components to exchange requests and information.

### Observed Example

The primary interface is enp1s0, which has the IPv4 address 172.30.1.2/24.

---

## Operating System

The operating system manages the resources of the server and provides an environment where applications can run.

### Importance

The operating system controls processes, memory, files, users, and network services. It acts as the main software layer that coordinates the resources of the server.

### Observed Example

The virtual environment runs Ubuntu 24.04.4 LTS with kernel version 6.8.0-138-generic.

---

## Component Interaction

These components depend on one another to support a cloud workload. The operating system manages the infrastructure, compute resources process application tasks, storage keeps information, and networking connects the system with users and other resources.
