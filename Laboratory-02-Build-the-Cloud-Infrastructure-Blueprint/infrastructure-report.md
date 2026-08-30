# Infrastructure Investigation Report

## System Information

| Resource         | Observed Result                               |
| ---------------- | --------------------------------------------- |
| Operating System | Ubuntu 24.04.4 LTS                            |
| Kernel Version   | 6.8.0-138-generic                             |
| CPU Model        | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| Processor Cores  | 1                                             |
| Memory           | 1.9 GiB                                       |
| Hostname         | ubuntu                                        |

### Explanation

The Linux environment examined during the activity is based on Ubuntu 24.04.4 LTS. The virtual server has one processor core and about 1.9 GiB of available memory. The kernel acts as the main connection between the operating system and the virtual hardware resources.

## Network Information

| Network Resource    | Observed Result |
| ------------------- | --------------- |
| Main Interface      | enp1s0          |
| Connection Status   | UP              |
| IPv4 Address        | 172.30.1.2/24   |
| Loopback Interface  | lo              |
| Loopback Address    | 127.0.0.1/8     |
| Container Interface | docker0         |
| Container Address   | 172.17.0.1/16   |

### Explanation

The enp1s0 interface is the active network interface of the environment. It provides the primary network connection for the virtual server. The loopback interface supports communication within the system itself, while the docker0 interface is associated with container networking.

## Storage Information

| Storage Device | Type | Total Size | Used | Available | Usage | Mounted At |
| -------------- | ---- | ---------: | ---: | --------: | ----: | ---------- |
| /dev/vda1      | ext4 |        19G | 5.4G |       13G |   30% | /          |
| /dev/vda16     | ext4 |       881M | 117M |      703M |   15% | /boot      |
| /dev/vda15     | vfat |       105M | 6.2M |       99M |    6% | /boot/efi  |

### Explanation

The primary storage device is /dev/vda1, which contains the root filesystem. It uses the ext4 filesystem and provides the largest storage capacity in the environment. Additional partitions are used for boot files and EFI-related system files.

## Overall Observation

The KillerCoda environment demonstrates the basic resources found in a cloud server. CPU and memory provide processing capability, storage holds the operating system and files, and networking allows communication with other systems. Linux manages these resources and provides the operating environment for workloads.
