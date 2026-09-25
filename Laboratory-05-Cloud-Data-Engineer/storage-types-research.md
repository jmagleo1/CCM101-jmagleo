# Storage Types Research

Cloud storage provides different ways to store and manage data depending on the needs of an application. The three primary types of cloud storage are Block Storage, File Storage, and Object Storage.

| Storage Type       | Description                                                                                                                    | Primary Use Case                                                                                  | Cloud Provider Example              |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- | ----------------------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be accessed individually. It works like a virtual hard drive attached to a server.   | Best for virtual machines, databases, and applications that need fast and consistent disk access. | **AWS EBS (Elastic Block Store)**   |
| **File Storage**   | Stores data as files organized into folders and directories. Multiple systems can access the same file storage over a network. | Best for shared files, documents, and applications that need a traditional file system.           | **AWS EFS (Elastic File System)**   |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. Objects are stored inside containers called buckets.    | Best for images, videos, backups, documents, and other large amounts of unstructured data.        | **AWS S3 (Simple Storage Service)** |

## Why Object Storage is Best for the Client

Object Storage is the best choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as user-uploaded images. It can scale as the number of photos increases and keeps the files separate from the web server, making it suitable for storing millions of user-uploaded images.

