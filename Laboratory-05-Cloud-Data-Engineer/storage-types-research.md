# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type   | Description                                                                                      | Primary Use Case                                                            | Cloud Provider Example |
| -------------- | ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------- | ---------------------- |
| Block Storage  | Stores data in fixed-size blocks that can be attached to a virtual machine and used like a disk. | Operating systems, databases, and applications that need fast disk access.  | AWS EBS                |
| File Storage   | Stores data in files and folders that can be accessed through a shared file system.              | Shared documents, application files, and workloads that need shared access. | AWS EFS                |
| Object Storage | Stores data as objects together with metadata and unique identifiers.                            | Images, videos, backups, documents, and other unstructured data.            | AWS S3                 |

## Why Object Storage is Suitable for User-Uploaded Images

Object Storage is a good choice for storing millions of user-uploaded images because it is designed for large amounts of unstructured data. Images can be stored as individual objects and accessed when needed without depending on the file system of the web server.
