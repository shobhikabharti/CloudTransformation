
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
26. **Bigquery** is used for data warehouse migration   
27. **Bigtable** is NoSQL based service  
28. **Cloud SQL** is a managed relational database service suitable for ***regionally*** used applications
29. **Cloud Spanner** is also a managed relational database, but it is designed for ***multi-region and global applications***  
30. **Cloud Dataproc** is a managed Spark/Hadoop service, not a relational database  
31. Bigtable does not support SQL. Cloud SQL and Cloud Spanner support SQL but are designed for transaction processing, not analytical applications like data warehouses.**Bigquery** is developed for that purpose
32. Bigtable is a NoSQL wide-column database optimized for heavy reads and writes. On the other hand, BigQuery is an enterprise data warehouse for large amounts of relational structured data 

**GCP NoSQL Databases  
Keymemory store - Cloud Memorystore  
Document store - Cloud Firestore  
Wide-column store - Cloud Bigtable**

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


