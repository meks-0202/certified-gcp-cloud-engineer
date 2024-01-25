## Cloud Dataflow
- A fully managed, serverless service for real-time stream processing and batch processing of data. It provides a unified programming model for building data pipelines and can handle large volumes of data with automatic scaling.
- Cloud Bigtable is purpose-built for high-volume data streams and provides the low-latency and high-throughput needed for IoT data analytics.

## Pub/Sub
- Pub/sub does not offer built-in real-time stream processing and analytics capabilities. Cloud Pub/Sub is a messaging service that enables asynchronous communication between independent components of an application. While it can handle message streaming.

## App Engine
- Google App Engine Standard Environment is designed for stateless applications and automatically scales based on traffic, meeting both requirements.
- App Engine is a fully managed platform-as-a-service (PaaS) offering that provides automatic scaling and load balancing capabilities for web applications. It abstracts away infrastructure concerns, allowing developers to focus on writing code rather than managing servers.

## Could Function
Cloud Functions scale automatically, including down to zero, making it cost-effective for sporadic traffic patterns.

## Compute Engine
- Compute Engine offers virtual machines (VMs) that can be customized and controlled directly by the user. While it provides flexibility and control over the infrastructure, it requires manual scaling and load balancing configuration.

## K8s
-  In Kubernetes, a pod represents the smallest deployable unit of computing that you can create and manage in a cluster. A pod is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers. Containers within the same pod have a few key advantages:

Shared Network Namespace: Containers in the same pod can communicate with each other using localhost, which provides minimal latency.

Shared Storage: They can also share volumes, providing an easy way to share data between containers.

## Deployment Manager
- deployment manager is the Infrastructure as a code tool for GCP. Deployment Manager is the recommended method for dynamically provisioning VMs on Compute Engine according to Google's best practices. Deployment Manager allows you to describe and provision all the resources necessary for your application in a declarative format, using YAML or Python templates. It provides a consistent and reproducible way to create and manage your infrastructure. By defining the VM specifications in a configuration file and using Deployment Manager, you can easily create and manage multiple VM instances in an automated and scalable manner.

## Cloud Spanner
- Cloud Spanner is a fully managed relational database with unlimited scale, strong consistency, and up to 99.999% availability.

- Additional note: Cloud Spanner is a fully managed, mission-critical, relational database service that offers transactional consistency at a global scale, automatic, synchronous replication for high availability, and support for two SQL dialects: Google Standard SQL (ANSI 2011 with extensions) and PostgreSQL.

- It provides strong consistency and ensures that users from all over the world see the exact same data with minimal latency. It automatically replicates data across multiple regions, making it highly available and reducing latency for users.

## Cloud Identity Proxy
- Cloud Identity Aware Proxy can be used to enable access to VMs that do not have external IP addresses or do not permit Direct Access over the internet. Configuring Cloud Identity-Aware Proxy for SSH and TCP resources allows you to access the VMs using an SSH client over the internet without having to configure any specific network-related changes. This option ensures that no additional configuration is required for new VMs added to the project.

## Random
- External Network Load Balancer exposes the traffic to the internet and it supports UDP. Setting up an External Network load balancer allows for load balancing of UDP traffic and can provide a single IP address for external access to the backend servers.
- For MySQL  You must enable binary logging to use point-in-time recovery. Enabling binary logging causes a slight reduction in write performance.
-  "The application holds the full database in-memory for fast data access", so it'll be more appropriate to use memory-optimized machine types. The M1 machine type in Compute Engine is designed for memory-intensive workloads. It provides a high memory-to-CPU ratio, making it suitable for applications that need to store the full database in memory to minimize latency.
-  If a data Studio report is broken then it probably means that the data which it is connected to is broken, so the first thing to look at is BigQuery. Going to the BigQuery interface allows you to review the nightly job that recalculates the daily summary and overwrites the table. By reviewing the job, you can look for any errors or issues that may have caused the charts in the Data Studio dashboard to break. This is the most direct and relevant method to debug the issue.
-  
