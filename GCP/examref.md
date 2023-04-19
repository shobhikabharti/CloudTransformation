
## Exam Refresher

1. role/owner : by default role granted to member, other roles include 'roles/editor', 'roles/viewer', and 'roles/browser'    
2. DNS settings is used for *Cloud identity verification record for your domain*   
3. Shielded VM : saves from compromised by a rootkit or other kernel-level **malware**  
4. Premptible VM : Preemptible VMs always stop after 24 hours. Suitable for batch jobs and fault-tolerant workloads  
5. Spot VM : highly affordable compute instances suitable for batch jobs and fault-tolerant workloads (no limit on lifetime)  
6. Clone persistent disk : Zone , region, and disk type has to be same  
7. Unmanaged instance group : useful for grouping together VMs that require individual configuration settings or tuning. e.g., for nodes in the cluster are heterogeneous in nature  
8. Managed instance group (MIG) : require consistent configuration settings based on an instance template  
9. Instance template : instance template is needed to enable Compute Engine to automatically add instances to a managed instance group  
10. Sole-tenant nodes : keep your VMs physically separated from VMs in other projects, or to group your VMs together on the same host hardware  
11. Persistent Disk : PD volumes provide high-performance and redundant network storage. By default, VMs use zonal persistent disks, and store your data on volumes located within a single zone, such as us-west1-c  
12. Hyperdisk : Designed for the most demanding mission-critical applications, max. 8 Hyperdisk volumes per VM instance. It  is priced by provisioned capacity and IOPS  
13. Local SSDs : Unlike Persistent Disks, Local SSDs are physically attached to the server that hosts your VM instance. This tight coupling offers superior performance, very high input/output operations per second (IOPS), and very low latency compared to persistent disks ... fixed 375 GB capacity for each device that you attach to the instance .. RAID on Linux  
14. Containers : Both managed Cloud Run services and GKE clusters can be created and managed completely from the console as well as from the command line.   

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


