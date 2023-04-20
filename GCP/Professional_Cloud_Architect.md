# Professional Cloud Architect

<p align="center">
  <img src ="/Content/rainbow.png" />
</p>

## Day 1 & Day 2
#### APR 17 2023, APR 18, 2023 > 15 days PCA Training starts today, prerequisites hands-on on ACE https://github.com/shobhikabharti/CloudTransformation/blob/main/GCP/README.md  
The [Professional Cloud Architect](https://cloud.google.com/architecture) certification exam assesses your ability to : 

   1. Design and plan a cloud solution architecture 
   2. Manage and provision the cloud solution infrastructure 
   3. Design for security and compliance  
   4. Analyze and optimize technical and business processes  
   5. Manage implementations of cloud architecture  
   6. Ensure solution and operations reliability  

  Before marching on the journey, start with the Sketch Note by Priyanka Vergadia and keep it handy before exam https://github.com/priyankavergadia/GCPSketchnote  
  If confused, check recommendations on Google Cloud   
  
  Quickstart https://cloud.google.com/docs/get-started/  
  Google Cloud Architecture Framework https://cloud.google.com/architecture/framework   
  Cloud Architecture Center https://cloud.google.com/architecture/  
  Infrastructure Modernization https://cloud.google.com/solutions/infrastructure-modernization/  
  Application Modernization https://cloud.google.com/solutions/application-modernization/  
  DevOps https://cloud.google.com/devops  
  Security https://cloud.google.com/solutions/security/  
  Databases https://cloud.google.com/solutions/databases/  
  Artificial Intelligence https://cloud.google.com/solutions/ai/  
  Smart Analytics https://cloud.google.com/solutions/smart-analytics/  
  Industry Solutions https://cloud.google.com/solutions/#industry-solutions  
  Cloud Solutions (Small Businesses) https://cloud.google.com/solutions/#role-based-solutions-smb  
  Compliance as Code https://cloud.google.com/solutions/risk-and-compliance-as-code  
  
  #### Compute Engine 

  Virtual Machine Instances https://cloud.google.com/compute/docs/instances  
  Machine types https://cloud.google.com/compute/docs/machine-resource  
  Images https://cloud.google.com/compute/docs/images   
  Pricing https://cloud.google.com/compute/all-pricing  
  Storage Options https://cloud.google.com/compute/docs/disks  
  Spot https://cloud.google.com/compute/docs/instances/spot  
  Preemptible https://cloud.google.com/compute/docs/instances/preemptible  
  Snapshot https://cloud.google.com/compute/docs/disks/snapshots  
  Migration https://cloud.google.com/migrate/virtual-machines  
  Shielded VMs https://cloud.google.com/compute/shielded-vm/docs/shielded-vm  
  Sole Tenant Node Type https://cloud.google.com/compute/docs/nodes/sole-tenant-nodes, https://cloud.google.com/blog/products/gcp/introducing-sole-tenant-nodes-for-google-compute-engine  
  Plan for the Bare Metal Solution https://cloud.google.com/bare-metal/docs/bms-planning   
  
  #### VPC 
  
  Best practices and reference architectures for VPC design https://cloud.google.com/architecture/best-practices-vpc-design  
  VPC https://cloud.google.com/vpc/docs/vpc  
  Regions & Zones https://cloud.google.com/compute/docs/regions-zones  
  Subnets https://cloud.google.com/vpc/docs/subnets, three types of subnets https://k21academy.com/google-cloud/google-cloud-vpc/     
  Routes https://cloud.google.com/vpc/docs/routes  
  IP Addresses https://cloud.google.com/vpc/docs/ip-addresses, Internal vs External IPs    
  Connect https://cloud.google.com/vpc/docs/private-service-connect  
  VPC Flow logs https://cloud.google.com/vpc/docs/flow-logs  
  Firewall Rule https://cloud.google.com/vpc/docs/firewalls  
  Firewall Policies https://cloud.google.com/vpc/docs/firewall-policies-overview  
  Hierarchical Firewall Policies https://cloud.google.com/vpc/docs/firewall-policies  
  Security Whitepaper https://cloud.google.com/docs/security  
  Multiple interfaces https://cloud.google.com/vpc/docs/multiple-interfaces-concepts, https://cloud.google.com/vpc/docs/create-use-multiple-interfaces  
  Network Pricing https://cloud.google.com/vpc/network-pricing  


| Internal IP | External IP |
| --- | --- |
| Allocated from subnet range to VMs by DHCP | Bring your own IP address (BYOIP). Assigned from pool (ephemeral) |
| Alternatively, can reserve (static) internal IP address | Alternatively, can reserve (static) external IP address |

#### Cloud NAT   
Multiple VPC Networks  
https://docs.google.com/document/d/1Pjvk8I4pQj8gmg5NqwoaVJyFufYaOx8fLiCj5wK8YrI/edit  


Public IPs are not attached to NICs.  

<br/>
<p>
  <img src="/Content/compute.svg"/>
</p>
<br/>

Vertex AI Product Example https://cloud.google.com/vertex-ai/docs   

## Day 3
#### 19 APR 2023  

Horizontal vs Vertical scaling https://www.geeksforgeeks.org/horizontal-and-vertical-scaling-in-databases/, https://openmetal.io/docs/edu/openstack/horizontal-scaling-vs-vertical-scaling/   
Compute Engine Disk Snapshots (Create) https://cloud.google.com/compute/docs/disks/create-snapshots, https://cloud.google.com/compute/docs/disks/scheduled-snapshots    
Delete a Snapshot https://cloud.google.com/sdk/gcloud/reference/compute/snapshots/delete, https://cloud.google.com/sdk/gcloud/reference/compute/snapshots/delete  
Migrate VMs https://cloud.google.com/architecture/migrating-vms-migrate-for-compute-engine-getting-started  
Migrate Containers https://cloud.google.com/architecture/migrating-vms-to-containers-with-migrate-for-anthos  
Migrate kubernetes to GKE https://cloud.google.com/architecture/migrating-containers-kubernetes-gke  
Migrate monolithic to microservices https://cloud.google.com/architecture/migrating-a-monolithic-app-to-microservices-gke  
Migration in Real Environment https://cloud.google.com/architecture/migrating-containers-multi-cluster-gke-ingress-services  

Components in question GKE, Compute Engine for GKE worker nodes, Cloud Load Balancing, Virtual Private Cloud external static IP addresses, Multi Cluster Ingress, Cloud DNS, Cloud Storage  

Steps in Migration:  
- Provision a GKE cluster to simulate the source environment  
- Provision multiple GKE clusters to simulate the target environment  
- Deploy the example workloads that are provided in this tutorial  
- Configure Multi Cluster Service Discovery and Multi Cluster Ingress  
- Expose the example workloads with Multi Cluster Ingress  
- Deploy and use Multi Cluster Service Discovery  
- Switch traffic to the target environment   
- Decommission the source environment  

Before you begin, a Google Cloud organization in which you have the following Identity and Access Management (IAM) roles:
- Project Creator role (roles/resourcemanager.projectCreator)  
- Billing Account Administrator role (roles/billing.admin)  
- An active billing account  

Classful network https://en.wikipedia.org/wiki/Classful_network  
Classless network https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing    
Create custom image https://cloud.google.com/compute/docs/images/create-custom   
Base images https://cloud.google.com/software-supply-chain-security/docs/base-images  
Extra https://killercoda.com/   
Cloud block storage options cheat sheet https://cloud.google.com/blog/topics/developers-practitioners/google-cloud-block-storage-options-cheat-sheet  
Youtube link (Strorage & Workloads) https://www.youtube.com/watch?v=-Fkgp0pkSdc  
**Persistent Disk** https://cloud.google.com/compute/docs/disks  
Backup VMs/Machine Images https://cloud.google.com/compute/docs/machine-images  
Backup Disks/Snapshots https://cloud.google.com/compute/docs/disks/snapshots, https://cloud.google.com/compute/docs/disks/create-snapshots  
Sole tenant nodes https://cloud.google.com/compute/docs/nodes/sole-tenant-nodes, https://cloud.google.com/blog/products/gcp/introducing-sole-tenant-nodes-for-google-compute-engine  
Shared resources (VPC, Disks) https://cloud.google.com/vpc/docs/shared-vpc, https://cloud.google.com/vpc/docs/provisioning-shared-vpc, https://cloud.google.com/compute/docs/disks/sharing-disks-between-vms  
Caching https://cloud.google.com/storage/docs/caching, https://cloud.google.com/memorystore  
Filestore https://cloud.google.com/filestore, https://cloud.google.com/filestore/docs/overview, https://cloud.google.com/filestore/docs/networking   
Workloads https://cloud.google.com/compute/docs/tutorials/basic-webserver-apache, https://cloud.google.com/compute/docs/instances/sql-server/setup-mysql, https://cloud.google.com/compute/docs/containers   
Load Testing https://cloud.google.com/architecture/distributed-load-testing-using-gke   
Monitor (View Logs) https://cloud.google.com/compute/docs/logging/audit-logging, https://cloud.google.com/compute/docs/logging/usage-export  
VM Operations List -- gcloud compute operations list --filter="zone:(us-central1-c)"  
Monitor https://cloud.google.com/compute/docs/disks/monitor-regional-persistent-disk-replica-state  
Autoscale https://cloud.google.com/compute/docs/autoscaler  
Load Balancing https://cloud.google.com/compute/docs/instance-groups/adding-an-instance-group-to-a-load-balancer  
Optimize VMs https://cloud.google.com/compute/docs/instances/apply-machine-type-recommendations-for-instances  
Optimize MIGs https://cloud.google.com/compute/docs/instance-groups/apply-machine-type-recommendations-managed-instance-groups  
Workload Performance https://cloud.google.com/compute/docs/instances/set-threads-per-core  
Network Bandwidth https://cloud.google.com/compute/docs/networking/configure-vm-with-high-bandwidth-configuration  

*An ephemeral IP address is an IP address that doesn't persist beyond the life of the resource. For example, when you create an instance or forwarding rule without specifying an IP address, Google Cloud automatically assigns the resource an ephemeral IP address. In general, the ephemeral IP address is released if you stop or delete the resource. Reserving a static IP address assigns the address to your project until you explicitly release it. This is useful if you are dependent on a specific IP address for your service and need to prevent another resource from being able to use the address. Static addresses are useful if you need to move an IP address from one Google Cloud resource to another. Internal and external IP addresses can be ephemeral or static, with the following exceptions: - Regional internal IPv6 addresses are ephemeral only. Static regional external IPv6 addresses are available in Preview only.*

## Day 4
#### 20 APR 2023  

#### Cloud Storage 

Object Store vs. Block Store In Object stoarge, Indexing rigourously neeeded, metadata indexes on object id everything to expedite the search whereas block store is needed in ... Object (Standard, Nearline, Coldline, Archive)  
Introduction https://cloud.google.com/storage/docs/introduction  
Storage Transfer Options https://cloud.google.com/storage-transfer/docs/transfer-options  
Filestore https://cloud.google.com/filestore/docs/overview  
Cloud SQL https://cloud.google.com/sql/docs/introduction  
Spanner https://cloud.google.com/spanner/docs/sql-best-practices  
Firestore https://cloud.google.com/firestore/docs/reference/rest  
Bigtable https://cloud.google.com/bigtable/docs/overview  
Bigquery https://cloud.google.com/bigtable/docs/overview  
Memorystore (In memory data / caching) https://cloud.google.com/memorystore/docs/redis/redis-overview, https://cloud.google.com/blog/products/databases/memorystore-for-redis  
Host a static website https://cloud.google.com/storage/docs/hosting-static-website  
Object lifecycle management https://cloud.google.com/storage/docs/lifecycle  
ACL https://cloud.google.com/storage/docs/access-control/lists, https://cloud.google.com/storage/docs/access-control/create-manage-lists  
Retention Policy https://cloud.google.com/storage/docs/bucket-lock  


*Hot data is for analysts who need their data to be subsecond/ high concurrency to help them answer real-time questions. Cold data commonly sits in your data warehouse and is used for reporting and planning. And warm data is a balance between the two*

## Day 5
#### 21 APR 2023  
## Day 6
#### 24 APR 2023  
## Day 7
#### 25 APR 2023  
## Day 8
#### 26 APR 2023  
## Day 9
#### 27 APR 2023  
## Day 10
#### 28 APR 2023  
## Day 11
#### 1 MAY 2023  
## Day 12
#### 2 MAY 2023  
## Day 13
#### 3 MAY 2023  
## Day 14
#### 4 MAY 2023  
## Day 15
#### 5 MAY 2023  
