
## Exam Refresher

1. **role/owner** : by default role granted to member, other roles include 'roles/editor', 'roles/viewer', and 'roles/browser'    
2. **DNS settings** is used for *Cloud identity verification record for your domain*   
3. **Shielded VM** : saves from compromised by a rootkit or other kernel-level **malware**  
4. **Premptible VM** : Preemptible VMs always stop after 24 hours. Suitable for batch jobs and fault-tolerant workloads  
5. **Spot VM** : highly affordable compute instances suitable for batch jobs and fault-tolerant workloads (no limit on lifetime)  
6. **Clone persistent disk** : Zone , region, and disk type has to be same  
7. **Unmanaged instance group** : useful for grouping together VMs that require individual configuration settings or tuning. e.g., for nodes in the cluster are heterogeneous in nature  
8. **Managed instance group (MIG)** : require consistent configuration settings based on an instance template  
9. **Instance template** : instance template is needed to enable Compute Engine to automatically add instances to a managed instance group  
10. **Sole-tenant nodes** : keep your VMs physically separated from VMs in other projects, or to group your VMs together on the same host hardware  
11. **Persistent Disk** : PD volumes provide high-performance and redundant network storage. By default, VMs use zonal persistent disks, and store your data on volumes located within a single zone, such as us-west1-c  
12. **Hyperdisk** : Designed for the most demanding mission-critical applications, max. 8 Hyperdisk volumes per VM instance. It  is priced by provisioned capacity and IOPS  
13. **Object storage-Standard buckets, Nearline (30), Coldline (90), and Archive (365)**. Widely used for disaster recovery because it takes practically no time to switch to a backup bucket to recover from a disaster.   
14. **Block storage—Persistent Disk and Local SSD**  
15. **File storage—Filestore** provides a cloud-based shared file system for unstructured data. It offers really low latency and provides concurrent access to tens of thousands of clients with scalable and predictable performance up to hundreds of thousands of IOPS, tens of GB/s of throughput, and hundreds of TBs. You can scale capacity up and down on-demand.   
16. **Local SSDs** : Unlike Persistent Disks, Local SSDs are physically attached to the server that hosts your VM instance. This tight coupling offers superior performance, very high input/output operations per second (IOPS), and very low latency compared to persistent disks ... fixed 375 GB capacity for each device that you attach to the instance .. RAID on Linux  
17. **Containers** : Both managed Cloud Run services and GKE clusters can be created and managed completely from the console as well as from the command line.   
18. **Shared VPC vs. VPC Peering** 2 peered VPC can not share the same subnet ranges, while VPC sharing is sharing the same subnets  
19. **Shared VPC** allows an organization to connect resources from multiple projects to a VPC  
20. **VPC Network Peering** connects two Virtual Private Cloud (VPC) networks so that resources in each network can communicate with each other  
21. **Cloud VPN** securely connects your peer network to your Virtual Private Cloud (VPC) network through an **IPsec** VPN connection.  Traffic traveling between the two networks is encrypted by one VPN gateway and then decrypted by the other VPN gateway. Each Cloud VPN tunnel can support up to 3 gigabits per second (Gbps) for the sum of ingress and egress traffic  
22. **VPNs deal with workflow security problems, VPCs deal with the workload**  
23. **Classic VPN and HA VPN** gateways use external (internet routable) IPv4 addresses. Only ESP, UDP 500, and UDP 4500 traffic is permitted to these addresses. Classic VPN gateways have a single interface, a single external IP address, and support tunnels that use static routing (policy-based or route-based) while HA VPN has dynamic routing  
24. **Dedicated Interconnect** provides a direct physical connection between your on-premises network and Google's network  
25. **Partner Interconnect** provides connectivity between your on-premises and VPC networks through a supported service provider  
26. **Bigquery** is used for ***data warehouse service***  
27. **Bigtable** is NoSQL based ***database service***  
28. **Cloud SQL** is a managed relational database service suitable for ***regionally*** used applications
29. **Cloud Spanner** is also a managed relational database, but it is designed for ***multi-region and global applications***  
30. **Cloud Dataproc** is a managed Spark/Hadoop service, not a relational database  
31. Bigtable does not support SQL. Cloud SQL and Cloud Spanner support SQL but are designed for transaction processing, not analytical applications like data warehouses.**Bigquery** is developed for that purpose
32. Bigtable is a NoSQL wide-column database optimized for heavy reads and writes. On the other hand, BigQuery is an enterprise data warehouse for large amounts of relational structured data 
33. **Cloud Pub/Sub** is a queuing service that is used to ingest data and store it until it can be processed  
34. **Cloud Data Fusion** is a managed service that is designed for building data transformation pipelines  
35. **Compute Engine** is not a managed service  
36. **Cloud Dataprep** is used to prepare data for analytics and machine learning   
37. **Cloud Build** is a service for creating container images  
38. **URL maps** specify direct requests to particular services  
39. **Routes** are used to specify paths to destination IP addresses outside a subnet  
40. **Firewall rules** control the flow of traffic on a network  
41. **Traces** are used to understand the performance characteristics of services in a distributed system  
42. **Internal TCP/UDP Load Balancing** is used for internal traffic, that is not from the internet  
43. **SSL Proxy, TCP Proxy, and Network TCP/UDP load balancing** are used with external traffic  
44. The correct way to enable Cloud Operations for GKE is to use the parameters --logging and --monitoring  
45. Kubernetes Engine collects log data written to standard output (STDOUT) and standard error (STDERR)  
46. ***A shared VPC allows projects to share a common VPC network. VPNs are used to link VPCs to on-premises networks. Routes and firewall rules are not sufficient for implementing a common VPC***
47. ***If the connected networks are in different organizations, they must use VPC Network Peering. VPC sharing is only available within a single organization. Firewall rule changes may be needed, but that is not sufficient. VPNs are used to connect GCP networks with on-premises networks***
48. Types of IP addresses: Regional and Global for both Internal and External IPs  
49. Session stickiness, also known as session persistence, refers to the process by which a load balancer establishes an affinity between a client and a specific network server for the duration of a session.  
50. Cookies are files created by websites that you go to. They save browsing information to make your online experience easier. With cookies, sites can keep you signed in, remember your site preferences, and give you locally relevant content.  
51. Signed cookies are an alternative to signed URLs. Signed cookies protect access when separately signing tens or hundreds of URLs for each user isn't feasible in your application. https://cloud.google.com/cdn/docs/overview
52. Inventing in **greenfield** refers to developing completely new applications or systems from scratch, without any dependencies on existing systems
53. When the organization would follow a **brownfield approach**, which involves modernizing or migrating the existing application to the cloud while retaining some of its components, functionality, or data. Brownfield modernization allows organizations to leverage their existing investments and assets while taking advantage of the benefits offered by the cloud environment.
54. **Cloud Logging** helps organizations analyze logs and provides tools for application troubleshooting. It allows users to collect, view, and analyze log data from various sources and gain insights into the performance and behaviour of their applications and infrastructure.
55. Moving from a tactical to a transformational cloud adoption approach requires shifting cloud security practices. Adopting a **zero-trust model** with multiple layers of network security is aligned with a transformational approach. A zero-trust model assumes that no user or network is inherently trusted and enforces strict access controls and verification mechanisms at each layer of the network. This approach provides enhanced security by minimizing the attack surface and reducing the risk of unauthorized access.  
56. **Recommendations AI** is a service that provides personalized product recommendations, not specifically focused on maintaining personalized dialog with customers.
57. **Contact Center AI** is a Google Cloud solution that enables organizations to build and deploy virtual contact centers with AI capabilities. It combines conversational AI, virtual agents, and live agent support to enhance customer interactions and improve operational efficiency. By using Contact Center AI, the customer service department can automate repetitive tasks, provide personalized responses, and streamline customer interactions, leading to increased operational efficiency while maintaining personalized dialog with customers.  
58. **Text-to-Speech** is a service that converts text into natural-sounding speech and is not specifically focused on maintaining personalized dialog with customers.  
59. **Cloud Identity** is an identity and access management service that helps organizations manage user identities and control access to resources. It does not directly address the goal of increasing operational efficiency and maintaining personalized dialog with customers.  
60. **Anthos** is a hybrid and multi-cloud platform that allows organizations to modernize their applications and manage infrastructure across different environments, including on-premises and multiple cloud providers. While it provides capabilities for managing infrastructure, it is not specifically focused on building autoscaling web applications without infrastructure management.  
61. **App Engine** is a fully managed platform-as-a-service (PaaS) offering on Google Cloud that allows organizations to build and deploy web applications without the need to manage infrastructure. App Engine automatically scales the application based on the incoming traffic, handling the infrastructure management tasks, such as provisioning resources, load balancing, and autoscaling, so that organizations can focus on developing their applications.  
62. **Compute Engine** is an Infrastructure as a Service (IaaS) offering from Google Cloud that provides virtual machines for organizations to run their workloads. While it can be used in hybrid cloud scenarios, it does not provide the specific capabilities required to build an application once and run it both on-premises and in the public cloud.  
63. **Apigee** is an API management platform that helps organizations design, secure, and analyze APIs. It does not directly address the requirement of building autoscaling web applications without infrastructure management.  
64. **AutoML** is a suite of machine-learning products that enable organizations to build custom machine-learning models with minimal coding. It is not specifically designed for building autoscaling web applications without infrastructure management.  
65. The organization should use the **Google Cloud Debugger to better understand the behavior of their code in production and identify hard-to-find programming errors**. The Cloud Debugger is a tool provided by Google Cloud that allows developers to inspect and debug the state of their applications at any point in time, without affecting its performance or availability. By setting breakpoints and capturing snapshots of the application's code and variables, developers can gain insights into the runtime behavior and identify issues that may be difficult to reproduce in development or testing environments.  
66. **Google Cloud Profiler** is a different tool that helps developers understand the performance characteristics of their applications. It provides insights into the CPU and memory usage of the application, helping to optimize its performance, but it doesn't specifically focus on identifying programming errors.  
67. **Cloud Monitoring** is a tool provided by Google Cloud that allows organizations to monitor the health, performance, and availability of their applications and infrastructure. While it provides valuable insights into the overall state of the system, it doesn't specifically address the task of identifying hard-to-find programming errors.  
68. **Google Cloud Trace** is a tool that helps developers analyze the latency of their applications and identify performance bottlenecks. It tracks the flow of requests through an application and provides detailed timing information, but it doesn't directly assist in identifying programming errors  
69. **Cloud Functions** is a serverless compute service that allows organizations to run code in response to events without the need to manage infrastructure. However, it does not specifically address the requirement of building an application once and running it both on-premises and in the public cloud.  
70. **Apigee** is an API management platform, and its main function is not to replicate tracking APIs but rather to provide features for API management, security, analytics, and reporting.  
71. **Security Command Center** is an effective way to identify virtual machines running vulnerable disk images. The Security Command Center provides comprehensive visibility into the security posture of your cloud resources, including virtual machines. It allows you to monitor and identify security vulnerabilities, such as outdated or vulnerable operating systems. By leveraging the Security Command Center, your organization can quickly identify virtual machines that do not have the latest security updates and take appropriate actions to mitigate the risk.
72. **Compliance Reports Manager** and downloading a recent PCI audit may provide information related to compliance with Payment Card Industry Data Security Standard (PCI DSS) requirements, but it may not specifically help identify virtual machines without the latest security updates. Compliance reports typically focus on adherence to specific regulatory standards rather than identifying individual vulnerabilities.  
73. Security Command Center to identify virtual machines started more than two weeks ago is not a reliable method for identifying virtual machines without the latest security updates. The age of a virtual machine does not necessarily indicate whether it has the latest security updates or is vulnerable to security vulnerabilities. It is possible for newer virtual machines to have outdated or vulnerable operating systems if proper updates have not been applied.   
74. Compliance Reports Manager and downloading a recent SOC 1 (Service Organization Control 1) audit report may provide insights into the effectiveness of controls related to financial reporting but does not directly address identifying virtual machines without the latest security updates. SOC 1 audits focus on the evaluation of internal controls related to financial reporting, rather than specifically assessing the presence of security vulnerabilities or outdated software versions.
75. 







**GCP NoSQL Databases  
Keymemory store - Cloud Memorystore  
Document store - Cloud Firestore  
Wide-column store - Cloud Bigtable**

**Shared VPC - common VPC n/w, single organization
VPN - On premises n/w
Peering - n/w between diff organizations**


- To get the information of source disk for each snapshot  
gcloud compute snapshots describe   

Both Ingress and Egress -> The priority of a firewall rule can range from 0 to 65535. The lower the number, the higher the priority. The default priority when you create a new rule is 1000.
Refer https://cloud.google.com/vpc/docs/firewalls 
<br/>
| Instance machine type | Maximum number of stateful connections |
| --- | --- |
| Shared-core machine types | 130,000 |
| Instances with 1–8 vCPUs | 130,000 connections per vCPU |
| Instances with more than 8 vCPUs | 1,040,000 (130,000×8) connections total |
<br/>

#### Terraform files

main.tf start every module  
network.tf, instances.tf, or loadbalancer.tf logical groupings of resources with their own files  
variables.tf declare all variables  
output.tf organize all outputs  
data.tf data sources (optional)  
dns.tf group resources by their shared purpose  

-- SERVICE-DIRECTORY/  
&emsp; -- OWNERS   
&emsp; -- modules/  
&emsp;&emsp; -- <service-name>/  
&emsp;&emsp; &emsp;&emsp; -- main.tf  
&emsp;&emsp; &emsp;&emsp; -- variables.tf  
&emsp;&emsp; &emsp;&emsp; -- outputs.tf  
&emsp;&emsp; &emsp;&emsp; -- provider.tf  
&emsp;&emsp; &emsp;&emsp; -- README   
&emsp;&emsp; -- ...other…  
&emsp; -- environments/  
&emsp;&emsp; -- dev/   
&emsp;&emsp; &emsp;&emsp; -- backend.tf  
&emsp;&emsp; &emsp;&emsp; -- main.tf  
&emsp;&emsp; -- qa/  
&emsp;&emsp; &emsp;&emsp; -- backend.tf  
&emsp;&emsp; &emsp;&emsp; -- main.tf  
&emsp;&emsp; -- prod/  
&emsp;&emsp; &emsp;&emsp; -- backend.tf  
&emsp;&emsp; &emsp;&emsp; -- main.tf  
  </br>

## Topics on GCPE

**Setting up a cloud solution environment**   
&emsp;&emsp; IAM, Cloud Identity, Resource hierarchy and policies, billing   
**Planning and configuring a cloud solution**  
&emsp;&emsp; Compute Services -> Compute Engine, Google Kubernetes Engine, Cloud Run, Cloud Functions  
&emsp;&emsp; Storage Service -> Cloud SQL, BigQuery, Firestore, Cloud Spanner, Cloud Bigtable  
&emsp;&emsp; Storage Options -> Zonal persistent disk, Regional balanced persistent disk, Standard, Nearline, Coldline, Archive  
&emsp;&emsp; Load balancing  
&emsp;&emsp; Cloud DNS  
**Deploying and implementing a cloud solution**  
&emsp;&emsp; Google Cloud events (e.g., Pub/Sub events, Cloud Storage object change notification events)  
&emsp;&emsp; Develop data solutions (e.g., Cloud SQL, Firestore, BigQuery, Cloud Spanner, Pub/Sub, Cloud Bigtable, Dataproc, Dataflow, Cloud Storage)  
&emsp;&emsp; Loading data (e.g., command line upload, API transfer, import/export, load data from Cloud Storage, streaming data to Pub/Sub)&emsp;&emsp;   
&emsp;&emsp; Creating a VPC with subnets (e.g., custom-mode VPC, shared VPC)  
&emsp;&emsp; Network configuration (e.g., internal-only IP address, Google private access, static external and private IP address, network tags)  
&emsp;&emsp; Firewall rules for a VPC (e.g., IP subnets, network tags, service accounts)  
**Ensuring successful operation of a cloud solution**  
&emsp;&emsp; Working with snapshots (e.g., create a snapshot from a VM, view snapshots, delete a snapshot)  
&emsp;&emsp; Working with images (e.g., create an image from a VM or a snapshot, view images, delete an image)  
&emsp;&emsp; Working with instance groups (e.g., set autoscaling parameters, assign instance template, create an instance template, remove instance group)  
&emsp;&emsp; Working with management interfaces (e.g., Google Cloud console, Cloud Shell, Cloud SDK)  
&emsp;&emsp; Managing GKE resources   
&emsp;&emsp; &emsp;&emsp; Viewing current running cluster inventory (nodes, pods, services)  
&emsp;&emsp; &emsp;&emsp; Browsing Docker images and viewing their details in the Artifact Registry  
&emsp;&emsp; &emsp;&emsp; Working with node pools (e.g., add, edit, or remove a node pool)  
&emsp;&emsp; &emsp;&emsp; Working with pods (e.g., add, edit, or remove pods)  
&emsp;&emsp; &emsp;&emsp; Working with services (e.g., add, edit, or remove a service)  
&emsp;&emsp; &emsp;&emsp; Working with stateful applications (e.g. persistent volumes, stateful sets)  
&emsp;&emsp; &emsp;&emsp; Managing Horizontal and Vertical autoscaling configurations  
&emsp;&emsp; &emsp;&emsp; Working with management interfaces (e.g., Google Cloud console, Cloud Shell, Cloud SDK, kubectl)  
&emsp;&emsp; Managing Cloud Run resources  
&emsp;&emsp; &emsp;&emsp; Adjusting traffic-splitting parameters  
&emsp;&emsp; &emsp;&emsp; Setting scaling parameters for autoscaling instances  
&emsp;&emsp; &emsp;&emsp; Determining whether to run Cloud Run (fully managed) or Cloud Run for Anthos  
&emsp;&emsp; Managing storage and database solutions  
&emsp;&emsp; &emsp;&emsp; Securing objects  
&emsp;&emsp; &emsp;&emsp; Setting object life cycle management policies for Cloud Storage buckets  
&emsp;&emsp; &emsp;&emsp; Executing queries to retrieve data from data instances (e.g., Cloud SQL, BigQuery, Cloud Spanner, Datastore, Cloud Bigtable)  
&emsp;&emsp; &emsp;&emsp; Estimating costs of data storage resources  
&emsp;&emsp; &emsp;&emsp; Backing up and restoring database instances (e.g., Cloud SQL, Datastore)  
&emsp;&emsp; &emsp;&emsp; Reviewing job status in Dataproc, Dataflow, or BigQuery  
&emsp;&emsp; Managing networking resources  
&emsp;&emsp; &emsp;&emsp; Adding a subnet to an existing VPC  
&emsp;&emsp; &emsp;&emsp; Expanding a subnet to have more IP addresses  
&emsp;&emsp; &emsp;&emsp; Reserving static external or internal IP addresses  
&emsp;&emsp; &emsp;&emsp; Working with CloudDNS, CloudNAT, Load Balancers and firewall rules  
&emsp;&emsp; Monitoring and logging  
&emsp;&emsp; &emsp;&emsp; Creating Cloud Monitoring alerts based on resource metrics  
&emsp;&emsp; &emsp;&emsp; Creating and ingesting Cloud Monitoring custom metrics (e.g., from applications or logs)  
&emsp;&emsp; &emsp;&emsp; Configuring log sinks to export logs to external systems (e.g., on-premises or BigQuery)  
&emsp;&emsp; &emsp;&emsp; Configuring log routers  
&emsp;&emsp; &emsp;&emsp; Viewing and filtering logs in Cloud Logging  
&emsp;&emsp; &emsp;&emsp; Viewing specific log message details in Cloud Logging  
&emsp;&emsp; &emsp;&emsp; Using cloud diagnostics to research an application issue (e.g., viewing Cloud Trace data, using Cloud Debug to view an application point-in-time)  
&emsp;&emsp; &emsp;&emsp; Viewing Google Cloud status  
**Configuring access and security**  
&emsp;&emsp;  Defining custom IAM roles (e.g., primitive, predefined and custom)  
&emsp;&emsp;  Managing service accounts. Tasks include:  
&emsp;&emsp;  &emsp;&emsp; Creating service accounts  
&emsp;&emsp;  &emsp;&emsp; Using service accounts in IAM policies with minimum permissions  
&emsp;&emsp;  &emsp;&emsp; Assigning service accounts to resources  
&emsp;&emsp;  &emsp;&emsp; Managing IAM of a service account  
&emsp;&emsp;  &emsp;&emsp; Managing service account impersonation  
&emsp;&emsp;  &emsp;&emsp; Creating and managing short-lived service account credentials  

