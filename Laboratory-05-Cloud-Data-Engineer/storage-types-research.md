
# Research: Types of Cloud Storage

## Overview

Cloud storage allows users and organizations to store data on remote servers that can be accessed through a network. The three primary types of cloud storage are Block Storage, File Storage, and Object Storage. Each type has different features and is designed for specific storage requirements.

## Comparison of Cloud Storage Types

| Storage Type | Description (How It Stores Data) | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Stores data in fixed-sized blocks, with each block managed separately. The blocks can be combined to form a storage volume. | Best for virtual machine disks, operating systems, and databases that require fast and consistent access to data. | AWS Elastic Block Store (EBS) |
| **File Storage** | Stores data as files organized into folders and directories using a hierarchical structure. | Best for shared files, team documents, content management, and applications that need shared file access. | AWS Elastic File System (EFS) |
| **Object Storage** | Stores data as individual objects containing the data itself, metadata, and a unique identifier. Objects are organized into containers called buckets. | Best for user-uploaded images, videos, backups, documents, and large amounts of unstructured data. | AWS Simple Storage Service (S3) |

## Client Explanation: Why Object Storage?

Object Storage is the best choice for storing user-uploaded images because it can handle millions of files efficiently and scale as the application grows. It also supports metadata, making images easier to organize and retrieve, while providing high durability and convenient access through APIs. This allows the application to store images separately from its main database without requiring a traditional file system.
