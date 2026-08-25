
# Cloud Provider Comparison

## Overview

AWS, Microsoft Azure, and Google Cloud Platform are public cloud platforms that provide the basic resources needed to build and operate applications. Their services have different names, but they perform similar roles, which makes it possible to compare their infrastructure offerings.

## Comparison of Core Infrastructure Services

| Infrastructure Component                 | AWS        | Microsoft Azure        | Google Cloud Platform       |
| ---------------------------------------- | ---------- | ---------------------- | --------------------------- |
| **Compute**                              | Amazon EC2 | Azure Virtual Machines | Compute Engine              |
| **Storage**                              | Amazon S3  | Azure Blob Storage     | Cloud Storage               |
| **Networking**                           | Amazon VPC | Azure Virtual Network  | Virtual Private Cloud (VPC) |
| **Identity and Access Management (IAM)** | AWS IAM    | Microsoft Entra ID     | Cloud IAM                   |

The service names above represent the main equivalent infrastructure offerings documented by the three providers. AWS uses EC2 for virtual computing and VPC for isolated networking, while Google Cloud provides Compute Engine and VPC for comparable purposes.

For storage, AWS S3, Azure Blob Storage, and Google Cloud Storage are designed to keep and manage data in the cloud. Their access-control systems also allow administrators to determine which users, applications, or services are allowed to use specific resources.

---

## Guide Questions

### 1. Which cloud provider offers the broadest range of services? Explain your answer.

Among the three providers, **AWS** is generally regarded as having one of the largest and most extensive cloud service portfolios. Its offerings cover many areas beyond basic infrastructure, including databases, analytics, security, application development, containers, and artificial intelligence.

### 2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?

I would choose **Microsoft Azure** for an organization that already depends heavily on Microsoft technologies. Azure works naturally with Microsoft's identity and enterprise ecosystem, making it easier to connect existing Microsoft-based systems with cloud resources.

### 3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?

**Google Cloud Platform** is a strong choice for AI, machine learning, and Kubernetes-related workloads. Google Cloud provides services for AI and ML development and offers Google Kubernetes Engine (GKE), while Kubernetes itself originated from Google's container-management work.

### 4. What similarities did you observe among the three cloud providers?

All three providers follow a similar basic cloud infrastructure model. Each one provides a way to run virtual machines, store data, create private or isolated networks, and control user permissions through identity and access-management features. AWS uses IAM policies for permissions, while Google Cloud also uses IAM roles and policies to control access to resources.

---

## Key Observation

The biggest difference between the providers is not the basic purpose of their infrastructure services but the way those services are designed, named, and integrated with their respective ecosystems. Learning the equivalent services across AWS, Azure, and Google Cloud helps cloud engineers move between platforms and choose the provider that fits a project's requirements.

## Official Documentation References

* [AWS Documentation](https://docs.aws.amazon.com/?utm_source=chatgpt.com)
* [Microsoft Azure Documentation](https://learn.microsoft.com/en-us/azure/?utm_source=chatgpt.com)
* [Google Cloud Documentation](https://cloud.google.com/docs?utm_source=chatgpt.com)
