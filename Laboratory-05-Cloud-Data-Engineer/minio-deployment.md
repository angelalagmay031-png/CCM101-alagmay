
# MinIO Object Storage Deployment

## Overview

This mission involved deploying MinIO, an S3-compatible object storage server, using Docker in the KillerCoda Ubuntu Playground. The server was configured with an API port and a web console port to manage buckets and uploaded objects.

## Docker Command Used

The following command was used to deploy the MinIO server:

```bash
docker run -d \
  -p 9000:9000 \
  -p 9001:9001 \
  --name minio-server \
  -e MINIO_ROOT_USER=cloudadmin \
  -e MINIO_ROOT_PASSWORD='CloudNova2026!' \
  cgr.dev/chainguard/minio server /data --console-address ":9001"
```

## Port Configuration

| Port | Purpose |
|---|---|
| 9000 | MinIO API port used by applications and S3-compatible clients |
| 9001 | MinIO Web Console used to manage buckets and objects |

The web console was accessed through port **9001** using the port-forwarding feature provided by the playground environment.

## Bucket Created

**Bucket Name:** `client-photos`

The `client-photos` bucket was created to store client-uploaded files. The MinIO Object Browser confirmed that the bucket was available and contained the uploaded file `Lagmay.txt`.

## Environment Variables (-e Flags)

The `-e` flags in the Docker command define environment variables inside the container.

- `MINIO_ROOT_USER=cloudadmin` sets the MinIO administrator username.
- `MINIO_ROOT_PASSWORD='CloudNova2026!'` sets the administrator password.

These environment variables configure the credentials used to authenticate with the MinIO server.

## Container Verification

The following command was used to verify that the container was running:

```bash
docker ps
```

The container appeared with the name `minio-server` and a status of `Up`.

An additional verification command was executed:

```bash
docker inspect -f '{{.State.Status}}' minio-server
```

The output was:

```text
running
```

## Conclusion

The MinIO object storage server was successfully deployed using Docker. The web console was used to create the `client-photos` bucket and upload a file, demonstrating the basic management of objects in an S3-compatible storage system.
