# MinIO Deployment

## Deployment Overview

For this laboratory, I deployed MinIO as an S3-compatible object storage server using Docker. The MinIO Web Console was accessed through port 9001.

## Docker Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```

## Port Configuration

| Port | Purpose           |
| ---- | ----------------- |
| 9000 | MinIO API         |
| 9001 | MinIO Web Console |

The MinIO Web Console was accessed using port **9001** through the KillerCoda port forwarding feature.

## Login Credentials

Username:

```text
cloudadmin
```

Password:

```text
CloudNova2026!
```

## Environment Variables

The `-e` flags define environment variables inside the Docker container.

`MINIO_ROOT_USER` sets the administrator username for MinIO.

`MINIO_ROOT_PASSWORD` sets the administrator password.

These variables allow the MinIO server to start with the specified administrator credentials.

## Bucket Created

The bucket created for this laboratory was:

```text
client-photos
```

## Uploaded Object

A sample file was uploaded to the `client-photos` bucket to verify that the object storage system was working correctly.

## Verification

The MinIO container was checked using Docker to confirm that the server was running successfully.

```bash
docker ps
```

The MinIO Web Console was then opened through port 9001, where the `client-photos` bucket and uploaded file were verified.
