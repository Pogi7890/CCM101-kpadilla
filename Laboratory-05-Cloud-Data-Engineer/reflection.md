# Mission Reflection

This laboratory helped me understand why object storage is useful for applications that need to handle a large amount of data. Object storage is suitable for millions of photos because each image can be stored as an individual object with its own metadata and identifier. Compared with using a traditional hard drive, object storage is designed to handle large amounts of unstructured data and can be accessed by applications when needed.

Docker made the MinIO deployment easier because I did not have to manually install and configure every part of the storage server. By using the Docker command, MinIO and its required environment were started inside a container. The port mappings and environment variables also allowed me to configure the service and access its web console.

A bucket is a storage container used to organize objects in object storage. In this activity, I created a bucket named `client-photos` and uploaded a sample file to it. This helped me understand how applications can organize uploaded files in cloud storage.

Large companies can protect object storage data by keeping multiple copies of their data and using different storage systems or physical locations. They can also use backups, replication, monitoring, and recovery systems so that data can still be available when a physical server fails. These methods reduce the risk of permanently losing important files.

My confidence in using the Linux command line is also improving. I was able to use commands to clone my repository, create directories, deploy a Docker container, and verify that the MinIO server was running. I also learned how Docker, port forwarding, and a web-based cloud storage interface can work together. This activity gave me more practical experience with deploying and documenting a cloud service.
