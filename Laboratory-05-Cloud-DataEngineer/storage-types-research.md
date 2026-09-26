# Storage Types Research

There are three common types of cloud storage: Block Storage, File Storage, and Object Storage. They are used for different purposes depending on what kind of data an application needs to store.

| Storage Type       | Description                                                                                               | Primary Use Case                                                                         | Cloud Provider Example |
| ------------------ | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------- |
| **Block Storage**  | Stores data in small blocks that can be accessed separately by a computer or server.                      | Commonly used for virtual machines, databases, and applications that need fast storage.  | AWS EBS                |
| **File Storage**   | Stores data as files inside folders and directories, similar to the storage system on a regular computer. | Useful for sharing files, documents, and other files between different users or systems. | AWS EFS                |
| **Object Storage** | Stores files as objects together with information or metadata about each file.                            | Useful for storing photos, videos, backups, documents, and other large amounts of data.  | AWS S3                 |

## Why Object Storage is Best for the Client

For the client's photo-sharing application, I think Object Storage is a suitable choice because the application will need to store a large number of photos. It can handle many files and can be expanded as more users upload their pictures. It also keeps the photos separate from the web server, which is useful because containers can be temporary.

## Summary

Block Storage is useful when a system needs storage that works like a regular hard drive. File Storage is better when files need to be arranged in folders and shared. Object Storage is useful for large amounts of files like photos and videos, which is why it fits the needs of the client's photo-sharing application.
