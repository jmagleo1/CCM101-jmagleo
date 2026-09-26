# MinIO Deployment Documentation

## Docker Command Used

docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
pgsty/minio server /data --console-address ":9001"

Note: Originally attempted with the official `minio/minio` and `quay.io/minio/minio` images, but both returned "unauthorized" / deprecated errors due to MinIO's recent licensing and distribution changes. Used `pgsty/minio`, a community-maintained fork, as a working alternative.

## Web Console Access

- Port used: **9001**
- Accessed via KillerCoda's Traffic/Ports panel (Custom Ports → entered 9001 → Access)

## Bucket Created

- Bucket name: **client-photos**

## Environment Variables (-e flags) Explanation

- `-e "MINIO_ROOT_USER=cloudadmin"` — sets the root/admin username used to log in to the MinIO server and web console. This acts as the master identity for managing the storage instance.
- `-e "MINIO_ROOT_PASSWORD=CloudNova2026!"` — sets the root/admin password paired with the username above. Together, these two environment variables authenticate the administrator and secure access to the server, preventing unauthorized users from managing buckets or objects.
