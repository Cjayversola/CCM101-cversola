# Types of Cloud Storage

Cloud storage has different types depending on how data is stored and accessed. The three common types are Block Storage, File Storage, and Object Storage.

## Comparison of Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks. The operating system can use these blocks like a hard drive. | Virtual machine disks and databases that need fast access. | AWS EBS |
| File Storage | Stores data as files organized into folders and directories. | Shared files, documents, and team folders. | AWS EFS |
| Object Storage | Stores data as objects with data, metadata, and a unique identifier. | Photos, videos, backups, and other unstructured data. | AWS S3 |

## Why Object Storage Is Best for User Photos

Object Storage is a good choice for the client's photo-sharing application because it can store large amounts of images as separate objects. It can also scale as more users upload photos. This makes it suitable for applications that need to store and access many images over time.
