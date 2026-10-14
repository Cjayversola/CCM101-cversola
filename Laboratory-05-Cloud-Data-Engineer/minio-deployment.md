# MinIO Deployment

## Deployment Steps

I deployed a MinIO object storage server using Docker in the KillerCoda Ubuntu Playground. The original image in the laboratory instructions could not be downloaded, so I used the Chainguard MinIO image instead.

## Docker Command

The following command was used to start the MinIO container:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
cgr.dev/chainguard/minio:latest server /data --console-address ":9001"
```

## Port Configuration

- **Port 9000:** MinIO API port.
- **Port 9001:** MinIO web console port.

I accessed the MinIO web console through port 9001 using the KillerCoda port access feature.

## Environment Variables

The `-e` option sets environment variables inside the container.

- `MINIO_ROOT_USER` sets the administrator username.
- `MINIO_ROOT_PASSWORD` sets the administrator password for this laboratory environment.

## Bucket Creation

I created a bucket named `client-photos` through the MinIO web console. This bucket is intended for storing the client's photos.

## Verification

I used the `docker ps` command to check whether the MinIO container was running and to verify its port mappings.
