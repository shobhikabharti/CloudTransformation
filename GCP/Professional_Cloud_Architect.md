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
  Test Prep https://www.examtopics.com/exams/google/professional-cloud-architect/view/  
  
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
Cloud Key Management Service https://cloud.google.com/kms/docs/cmek  
Encryption https://cloud.google.com/docs/security/encryption/customer-supplied-encryption-keys  
Cloud SQL read replicas https://cloud.google.com/sql/docs/postgres/replication/create-replica  

#### GCP NoSQL Databases
**Keymemory store - Cloud Memorystore   
Document store - Cloud Firestore  
Wide-column store - Cloud Bigtable**  

*Hot data is for analysts who need their data to be subsecond/ high concurrency to help them answer real-time questions. Cold data commonly sits in your data warehouse and is used for reporting and planning. And warm data is a balance between the two*

Lab : https://partner.cloudskillsboost.google/focuses/13477?parent=catalog  

## Day 5
#### 21 APR 2023  

#### IAM

Three kind of roles : Basic, predefined, custom 

Google Cloud Directory Sync https://support.google.com/a/answer/106368?hl=en, https://tools.google.com/dlpage/dirsync/, 
https://cloud.google.com/architecture/identity/federating-gcp-with-active-directory-synchronizing-user-accounts  
Cloud Identity https://cloud.google.com/identity/docs/overview  
Deny Policies https://cloud.google.com/iam/docs/deny-overview  
Service Account https://cloud.google.com/iam/docs/service-account-overview  
IAM FAQs https://cloud.google.com/iam/docs/faq    
Understanding Roles https://cloud.google.com/iam/docs/understanding-roles   
Predefined Roles https://cloud.google.com/iam/docs/understanding-roles#predefined_roles  
Basic Roles https://cloud.google.com/iam/docs/understanding-roles#basic  
Convenience Values https://cloud.google.com/storage/docs/access-control/iam#convenience-values  
IAM reference https://cloud.google.com/storage/docs/access-control/best-practices-access-control  
Using IAM permissions https://cloud.google.com/storage/docs/access-control/using-iam-permissions  
Granting & revoking https://cloud.google.com/iam/docs/granting-changing-revoking-access  
Using IAM permissions https://cloud.google.com/storage/docs/access-control/using-iam-permissions  
Recommendation for buckets https://cloud.google.com/policy-intelligence/docs/review-apply-role-recommendations-buckets  
Policy Intelligence https://cloud.google.com/policy-intelligence/docs/tools-overview  
Policy Simulator https://cloud.google.com/policy-intelligence/docs/iam-simulator-overview  
Recommender https://cloud.google.com/recommender/docs/overview    
Summary https://cloud.in28minutes.com/gcp-certification-google-cloud-iam, https://tutorialsdojo.com/google-cloud-identity-and-access-management-iam/  

## Day 6
#### 24 APR 2023  

#### Firewall 

About Firewalls https://cloud.google.com/firewall/docs/about-firewalls  
VPC Firewall https://cloud.google.com/firewall/docs/firewalls    
Network Tags https://cloud.google.com/firewall/docs/tags-firewalls-overview  
IAM Recommender https://cloud.google.com/policy-intelligence/docs/role-recommendations-overview  
Separation of Duties https://cloud.google.com/binary-authorization/docs/reference/organizational-and-iam-roles  
Principle of least privilege https://cloud.google.com/blog/products/application-development/least-privilege-for-cloud-functions-using-cloud-iam, https://cloud.google.com/blog/products/identity-security/dont-get-pwned-practicing-the-principle-of-least-privilege    
IAM best practices https://cloud.google.com/binary-authorization/docs/reference/organizational-and-iam-roles   

Best practce is to attach network tags to service accounts.   
Tags can be runnign when VM is running. Vm can be havign mutiple VMs.  
CIS Benchmarks for CPU Hardening or Cloud Hardening -> https://www.cisecurity.org/cis-benchmarks   

#### Hybrid Connectivity

Hybrid Connectivity https://cloud.google.com/network-connectivity/docs/how-to/choose-product, https://cloud.google.com/load-balancing/docs/negs/hybrid-neg-concept  
Cloud VPN https://cloud.google.com/network-connectivity/docs/vpn  
Cloud Interconnect https://cloud.google.com/network-connectivity/docs/interconnect  
Direct or Carrier Peering https://cloud.google.com/network-connectivity/docs/direct-peering, https://cloud.google.com/network-connectivity/docs/carrier-peering  
Cloud Router https://cloud.google.com/network-connectivity/docs/router/concepts/overview, https://cloud.google.com/network-connectivity/docs/router/pricing    
HA VPN https://cloud.google.com/load-balancing/docs/negs/hybrid-neg-concepts, https://cloud.google.com/network-connectivity/docs/vpn/how-to/creating-ha-vpn  
Dedicated Interconnect overview https://cloud.google.com/network-connectivity/docs/interconnect/concepts/dedicatedoverview  
Partner Interconnect overview https://cloud.google.com/network-connectivity/docs/interconnect/concepts/partner-overview  
Cloud Interconnect FAQ https://cloud.google.com/network-connectivity/docs/interconnect/support/faq 

#### Instance Groups 

Instance Groups https://cloud.google.com/compute/docs/instance-groups   
Instance Templates https://cloud.google.com/compute/docs/instance-templates  
Two Types -> Managed Instance groups (MIGs) or Unmanaged Instance groups  
MIGs https://cloud.google.com/compute/docs/instance-groups/creating-groups-of-managed-instances, https://cloud.google.com/compute/docs/instance-groups  
Stateful vs Stateless MIGs https://cloud.google.com/compute/docs/instance-groups/stateful-migs  
Unmanaged Instance groups https://cloud.google.com/compute/docs/instance-groups/creating-groups-of-unmanaged-instances, https://cloud.google.com/compute/docs/instance-groups  
Autoscaler https://cloud.google.com/compute/docs/autoscaler  
Scale In Policy https://cloud.google.com/compute/docs/load-balancing-and-autoscaling  
Further Autoscaler Options https://cloud.google.com/compute/docs/autoscaler/understanding-autoscaler-decisions  
Multiple Policies https://cloud.google.com/compute/docs/autoscaler/multiple-policies  
Autohealing https://cloud.google.com/compute/docs/instance-groups/autohealing-instances-in-migs  
<br/> 

|  | Stateless | Stateful |
| ---- |---- | ---- |
| Autoscaling | YES  | NO |
| Disk preservation | NO | YES |
| Auto-healing | YES | YES |
| Auto-updating | YES | YES |
| Load balancing | YES | YES |
| Multi-zone deployment | YES | YES | 
<br/>

#### Cloud Load Balancing 

What is Cloud Load Balancing https://cloud.google.com/blog/topics/developers-practitioners/what-cloud-load-balancing, https://cloud.google.com/load-balancing  
Video https://www.youtube.com/watch?v=h8EqM6Xt3MA, https://www.youtube.com/watch?v=0fQr7TRhnnU&list=PLTWE_lmu2InBzuPmOcgAYP7U80a87cpJd     
Corresponding blog https://cloud.google.com/blog/topics/developers-practitioners/what-cloud-load-balancing  
Backend Service https://cloud.google.com/load-balancing/docs/backend-service  
Instance group backend services https://cloud.google.com/load-balancing/docs/backend-service#instance_groups  
Health checks https://cloud.google.com/load-balancing/docs/backend-service#health-checks  
URL maps overview https://cloud.google.com/load-balancing/docs/url-map-concepts  
Premium Tier https://cloud.google.com/network-tiers/docs/overview#premium_tier  
Standard Tier https://cloud.google.com/network-tiers/docs/overview#standard_tier  
Network Service Tiers https://cloud.google.com/network-tiers
Network Service Tiers overview https://cloud.google.com/network-tiers/docs/overview  
Google Cloud networking in depth: Understanding Network Service Tiers (May 15, 2019) https://cloud.google.com/blog/products/networking/google-cloud-networking-in-depthunderstanding-network-service-tiers  
Google Cloud Armor https://cloud.google.com/armor  
Cloud DNS https://cloud.google.com/dns, https://cloud.google.com/dns/docs/overview  
DDoS Attack Protection -> Identity Aware Proxy (IAP) vs Cloud Armor  

<br/>
<p>
 <img src="/Content/clb_cover.jpeg"/>
</p> 
<br/>

## Day 7
#### 25 APR 2023  

#### Cloud CDN 

Lab : https://partner.cloudskillsboost.google/focuses/11633?parent=catalog, https://partner.cloudskillsboost.google/focuses/57169?parent=catalog, https://partner.cloudskillsboost.google/focuses/13312?parent=catalog   

Cloud Pub/Sub https://cloud.google.com/pubsub/docs/overview, https://cloud.google.com/pubsub  

BigQuery is part of Google Cloud’s comprehensive data analytics platform that covers the analytics value chain from Ingest >> process >> store >> advanced analytics and collaboration. BigQuery is deeply integrated with the GCP’s analytical and data processing offering, allowing customers to build an enterprise ready cloud native data warehouse.  
1. Cloud Pub/sub - Scaled messaging platform  
2. BigQuery Data Transfer Service - Ads data for marketing cloud   
3. Beam - Stream and batch processing with single programing model with Dataflow  
4. Dataproc - Managed Hadoop and Spark platform  
5. Dataprep - Analyst can now do data prep using visual tool  
6. Data Fusion - Fully managed, code-free data integration service to manage ETL/ELT pipelines and also track lineage of that data  
7. BigQuery cloud-native, highly scalable data warehouse  
8. Cloud Storage as your data lake for structured and unstructured data  
9. Vertex AI & Tensorflow for machine learning on top of data on BigQuery and Cloud Storage  
10. Looker Studio and Sheet for your analysis  

Google Cloud Big Data solutions are designed to help you transform your business and user experiences with meaningful data insights. It is an integrated, serverless platform. “Serverless” means you don’t have to provision compute instances to run your jobs. The services are fully managed, and you pay only for the resources you consume. The platform is “integrated” so Google Cloud data services work together to help you create custom solutions.  
Pub/Sub is an important building block for applications where data arrives at high and unpredictable rates, like Internet of Things systems. If you’re analyzing streaming data, Dataflow is a natural pairing with Pub/Sub.  
Pub/Sub also works well with applications built on Google Cloud’s compute platforms. You can configure your subscribers to receive messages on a “push” or a “pull” basis. In other words, subscribers can get notified when new messages arrive for them, or they can check for new messages at intervals.  
Dataproc is managed Hadoop. Dataproc is a fast, easy, managed way to run Hadoop, Spark, Hive, and Pig on Google Cloud. All you have to do is to request a Hadoop cluster. It will be built for you in 90 seconds or less, on top of Compute Engine virtual machines whose number and type you can control. If you need more or less processing power while your cluster’s running, you can scale it up or down. You can use the default configuration for the Hadoop software in your cluster, or you can customize it. And you can monitor your cluster using Operations.  

***HDFS***: Hadoop data file system. Cloud storage was originally named DFS (distributed file system)  
***HBase***: open-source, NoSQL, distributed big data store. Runs on top of HDFS. The GC equivalent is Bigtable  
***DFS*** - distributed file system = Cloud Storage  
***HA Dataproc*** has 3 masters (one is a witness); With no HA , have 1 master, no failover. All are in the same zone Primary workers can use autoscaling. Secondary workers are MIGs but do not scale. However if you tell Google you want 4 workers, it will try to keep 4 workers at al times. These can be spot VMs  
***HBASE*** - database that lives in HDFS. Equivalent to Cloud Bigtable  

Dataflow is a unified programming model and a managed service for developing and executing a wide range of data processing patterns including ETL, batch computation, and continuous computation.   

***ETL***: (extract/transform/load) pipelines to move, filter, enrich, shape data  
***Data analysis***: batch computation or continuous computation using streaming  
***Orchestration***: create pipelines that coordinate services, including external services  
Integrates with Google Cloud services like Cloud Storage, Pub/Sub, BigQuery, and Cloud Bigtable  
- Open source Java, Python SDKs  

**Dataflow** frees you from operational tasks like resource management and performance optimization.  
Dataflow features:   
***Resource Management***: Dataflow fully automates management of required processing resources. No more spinning up instances by hand.  
***On Demand***: All resources are provided on demand, enabling you to scale to meet your business needs. No need to buy reserved compute instances.  
***Intelligent Work Scheduling***: Automated and optimized work partitioning which can dynamically rebalance lagging work. No more chasing down “hot keys” or pre-processing your input data.  
***Auto Scaling***: Horizontal auto scaling of worker resources to meet optimum throughput requirements results in better overall price-to-performance.     
***Unified Programming Model***: The Dataflow API enables you to express MapReduce like operations, powerful data windowing, and fine grained correctness control regardless of data source.    
***Open Source***: Developers wishing to extend the Dataflow programming model can fork and or submit pull requests on the Java-based Dataflow SDK. Dataflow pipelines can also run on alternate runtimes like Spark and Flink.  
***Monitoring***: Integrated into the Cloud Console, Dataflow provides statistics such as pipeline throughput and lag, as well as consolidated worker log inspection—all in near-real time.  
***Integrated***: Integrates with Cloud Storage, Pub/Sub, Datastore, Cloud Bigtable, and BigQuery for seamless data processing. And can be extended to interact with others sources and sinks like Apache Kafka and HDFS.  
***Reliable & Consistent Processing***: Dataflow provides built-in support for fault-tolerant execution that is consistent and correct regardless of data size, cluster size, processing pattern or pipeline complexity.  

**Dataprep**  
- Allows data analysts, business analysts, data engineers, and data scientists to visually explore, clean, and prepare big data  
- Connects to BigQuery, Cloud Storage, Google Sheets, and hundreds of other cloud applications and traditional databases  
- Build on top of Dataflow and BigQuery   
- Data transformation and cleaning rules can easily translate into Dataflow jobs or BigQuery SQL statements  

***BigQuery is a fully managed data warehouse***  
- Provides near real-time interactive analysis of massive datasets (hundreds of TBs)  
- Query using SQL syntax (ANSI SQL 2011)  
- No cluster maintenance is required  
- Compute and storage are separated with a terabit network in between  
- You only pay for storage and processing used  
- Automatic discount for long-term data storage  

***BigQuery is NoOps***: there is no infrastructure to manage and you don't need a database administrator, so you can focus on analyzing data to find meaningful insights, use familiar SQL, and take advantage of our pay-as-you-go model. BigQuery is a powerful big data analytics platform used by all types of organizations, from startups to Fortune 500 companies.   
BigQuery’s features:    
***Flexible Data Ingestion***: Load your data from Cloud Storage or Datastore, or stream it into BigQuery at 100,000 rows per second to enable real-time analysis of your data.  
***Global Availability***: You have the option to store your BigQuery data in European locations while continuing to benefit from a fully managed service, now with the option of geographic data control, without low-level cluster maintenance.  
***Security and Permissions***: You have full control over who has access to the data stored in BigQuery. If you share datasets, doing so will not impact your cost or performance; those you share with pay for their own queries.  
***Cost Controls***: BigQuery provides cost control mechanisms that enable you to cap your daily costs at an amount that you choose. For more information, see Cost Controls.  
***Highly Available***: Transparent data replication in multiple geographies means that your data is available and durable even in the case of extreme failure modes.  
***Super Fast Performance***: Run super-fast SQL queries against multiple terabytes of data in seconds, using the processing power of Google's infrastructure. Fully Integrated In addition to SQL queries, you can easily read and write data in BigQuery via Dataflow, Spark, and Hadoop.  
***Connect with Google Products***: You can automatically export your data from Google Analytics Premium into BigQuery and analyze datasets stored in Google Cloud Storage, Google Drive, and Google Sheets.  
BigQuery can make Create, Replace, Update, and Delete changes to databases, subject to some limitations and with certain known issues.   

**Cloud Dataplex** is a fully managed and highly scalable data discovery and metadata management service  

Protect sensitive data with Data Loss Prevention https://cloud.google.com/dlp, https://cloud.google.com/blog/products/identity-security/modern-dlp-for-cloud-data-discovery   
Cloud Composer https://cloud.google.com/composer, https://cloud.google.com/composer/docs/concepts/overview, https://cloud.google.com/blog/topics/developers-practitioners/better-service-orchestration-workflows/  

Cloud Adoption Framework https://services.google.com/fh/files/misc/google_cloud_adoption_framework_whitepaper.pdf  


Containers https://www.docker.com, https://blog.purestorage.com/purely-informational/containerd-vs-docker-whats-the-difference   
Cloud Build documentation https://cloud.google.com/build/docs  
Cloud Build - Create a build configuration file (lots of good sections to review - look at the different topics on the left) https://cloud.google.com/build/docs/configuring-builds/create-basic-configuration  
Cloud Build Youtube video https://www.youtube.com/watch?v=2TZXSnCTd7E&list=PLTWE_lmu2InBzuPmOcgAYP7U80a87cpJd  
Cloud Source Repositories https://cloud.google.com/source-repositories  
Artifact Registry https://cloud.google.com/artifact-registry  
Container Registry https://cloud.google.com/container-registry  
Supported Build Steps https://cloud.google.com/build/docs/deploying-builds/deploy-cloud-run   
Write your own build steps https://cloud.google.com/build/docs/configuring-builds/use-community-and-custom-builders  
Continuous integration (CI) https://cloud.google.com/solutions/continuous-integration  
Building an automated serverless deployment pipeline with Cloud Build https://cloud.google.com/blog/topics/developers-practitioners/building-automated-serverless-deployment-pipeline-cloud-build  
What is Cloud Build? https://www.youtube.com/watch?v=Bvo6jzC3J_A  
Cloud Build - Create a build configuration file https://cloud.google.com/build/docs/configuring-builds/create-basic-configuration  
Cloud Run https://cloud.google.com/run/  
Knative https://knative.dev/  
Eventarc overview https://cloud.google.com/eventarc/docs/overview  

Google Kubernetes Engine  
Source: Kubernetes: Your Hybrid Cloud Strategy https://cloud.google.com/files/kubernetes-your-hybrid-cloud-strategy.pdf  
Cluster nodes Auto-upgrading https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-upgrades  
Cluster nodes Auto-repair https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-repair  
Types of clusters (Standard vs Autopilot, Regional vs Zonal) https://cloud.google.com/kubernetes-engine/docs/concepts/types-of-cluster  
AutoPilot https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview  
Overview of deploying workloads https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview  
gcloud container syntax https://cloud.google.com/sdk/gcloud/reference/container  
kubectl Cheat Sheet https://kubernetes.io/docs/reference/kubectl/cheatsheet/  
Services https://cloud.google.com/kubernetes-engine/docs/concepts/service  
Another overview: https://kubernetes.io/docs/concepts/services-networking/service/  
Exposing applications using services (includes add, edit and remove): https://cloud.google.com/kubernetes-engine/docs/how-to/exposing-apps  
GKE Services https://cloud.google.com/kubernetes-engine/docs/concepts/service  
About node pools https://cloud.google.com/kubernetes-engine/docs/concepts/node-pools  
Setting up a Private Kubernetes Cluster https://partner.cloudskillsboost.google/catalog_lab/908  
Configuring multidimensional Pod autoscaling https://cloud.google.com/kubernetes-engine/docs/how-to/multidimensional-pod-autoscaling  
Recommendations for planning, architecting, deploying, scaling, and operating large workloads on Google Kubernetes Engine (GKE) clusters https://cloud.google.com/kubernetes-engine/docs/best-practices/scalability  
https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/  
For more details on Requests and Limits, see: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/  
Cluster nodes scaling https://cloud.google.com/kubernetes-engine/docs/concepts/cluster-autoscaler  
Using node auto-provisioning https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-provisioning  
Enabling node auto-provisioning: https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-provisioning#enable  
Horizontal pod scaling https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler  
Custom and external metrics for Horizontal autoscaling workloads: https://cloud.google.com/kubernetes-engine/docs/concepts/custom-and-external-metrics  
Vertical pod scaling https://cloud.google.com/kubernetes-engine/docs/concepts/verticalpodautoscaler  
Youtube - Autoscaling with GKE https://www.youtube.com/watch?v=7naCIxIaV1M  
To run or not to run a database on Kubernetes: What to consider  
https://cloud.google.com/blog/products/databases/to-run-or-not-to-run-a-database-onkubernetes-what-to-consider  
Suggested tutorial: https://kubernetes.io/docs/tutorials/stateful-application/basic-stateful-set/  
Suggested Lab: Running a MongoDB Database in Kubernetes with StatefulSets https://partner.cloudskillsboost.google/catalog_lab/327  
Binary authorization https://github.com/grafeas/kritis/blob/master/docs/binary-authorization.md, https://cloud.google.com/binary-authorization/docs/cloud-build, https://cloud.google.com/binary-authorization/docs/vulnerability-scanning  
Anthos https://cloud.google.com/blog/topics/developers-practitioners/what-are-my-hybrid-and-multicloud-deployment-options-anthos   
Anthos overview   
Anthos blog https://cloud.google.com/blog/topics/developers-practitioners/how-does-anthos-simplify-hybrid-multicloud-deployments  
Youtube https://www.youtube.com/watch?v=FfJNAjoX3Uc&list=PLTWE_lmu2InBzuPmOcgAYP7U80a87cpJd  
Anthos Config Management: https://cloud.google.com/anthos/config-management, https://cloud.google.com/anthos/docs/concepts/overview#centralized_config_management   	
“What is Anthos” youtube video https://www.youtube.com/watch?v=Qtwt7QcW4J8&t=276s  
Anthos 101 learning series - Service Mesh https://www.youtube.com/watch?v=EDcy3KwV22o&t=294s, https://cloud.google.com/anthos/docs/concepts/overview#service_mesh_dashboard  
Deploying containers on VMs and MIGs https://cloud.google.com/compute/docs/containers/deploying-containers  
Containers on Compute Engine https://cloud.google.com/compute/docs/containers  
Limitation: only 1 container per VM: https://cloud.google.com/compute/docs/containers/deploying-containers#limitations  

***To run more than one container per VM, use Google Kubernetes Engine***  https://cloud.google.com/blog/topics/developers-practitioners/where-should-i-run-my-stuff-choosing-google-cloud-compute-option  

Cloud Functions https://cloud.google.com/functions  
Cloud Functions Overview https://cloud.google.com/functions/docs/concepts/overview  
Cloud Functions Lab https://partner.cloudskillsboost.google/catalog_lab/924  
App Engine cheat sheet https://cloud.google.com/blog/topics/developers-practitioners/ultimate-app-engine-cheat-sheet  
App Engine documentation https://cloud.google.com/appengine/docs/  
App Engine Standard https://cloud.google.com/appengine/docs/standard/  
App Engine Flexible https://cloud.google.com/appengine/docs/flexible/  
When should you choose Standard vs Flexible? https://cloud.google.com/appengine/docs/the-appengine-environments  
App Engine https://partner.cloudskillsboost.google/catalog_lab/1161  


Nintendo: Build a new general-purpose game server using Google Kubernetes Engine, Cloud Spanner, etc. https://cloud.google.com/blog/ja/topics/customers/nintendo-new-game-servers-built-with-gke-cloud-spanner?hl=ja  
Mahindra Reimagened https://cloud.google.com/blog/products/infrastructure/how-mahindra-reimagined-the-suv-buying-process-with-google-cloud

## Day 8
#### 26 APR 2023  

Using Pub/Sub with Cloud Run tutorial https://cloud.google.com/run/docs/tutorials/pubsub#run_pubsub_server-java  
Queue Tutorial https://cloud.google.com/tasks/docs/add-task-queue  
Cloud Function timeout https://cloud.google.com/functions/docs/configuring/timeout  
Kubernetes Quest https://www.cloudskillsboost.google/quests/29  

Other Google Enterprise API  

1. Cloud Build API - Continuously build, test, and deploy  
2. Cloud DNS API - Highly Available Global DNS Network  
3. Compute Engine API  
4. Artifact Registry API - Highly Available APIs  
5. Bare Metal Solution API - Provides ways to manage Bare Metal Solution hardware installed in a regional extension located near…  
6. Kubernetes Engine API - Builds and manages container-based applications, powered by the open source Kubernetes technology  

Node Pools https://cloud.google.com/kubernetes-engine/docs/concepts/node-pools  

Autoscaling Strategies :   
Horizontal Pod Autoscaler  https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler  
Vertical Pod Autoscaler  https://cloud.google.com/kubernetes-engine/docs/concepts/verticalpodautoscaler  
Cluster Autoscaler  https://cloud.google.com/kubernetes-engine/docs/concepts/cluster-autoscaler, https://cloud.google.com/kubernetes-engine/docs/how-to/cluster-autoscaler    
Node Auto Provisioning  https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-provisioning   

## Day 9
#### 27 APR 2023  

Docker images are lightweight, preconfigured virtual environments used to run our application. The images include the software required to run the containerized application. The applications are deployed inside the Docker image.  

Cloud Logging and Cloud Monitoring are the built-in logging and monitoring solutions for Google Cloud. Google Cloud’s operations suite offers a fully managed logging, metrics collection, monitoring, dashboarding, and alerting solution that watches all sides of your hybrid or multi-cloud network. It’s the ideal solution for customers wanting a single, easy to configure, powerful cloud-based observability solution that also gives you a single pane of glass dashboard to monitor all of your environments.  

Deploying containers on VMs and MIGs https://cloud.google.com/compute/docs/containers/deploying-containers  

Cloud Build functions similarly to Docker in that it accepts code and configuration and builds containers (among other things). Cloud Build offers many features and services that are geared towards professional development. It is designed to fit into a continuous development / continuous deployment workflow and can scale to handle many application developers working on and continuously updating a live global service.  

Cloud Build executes your build as a series of build steps, where each build step is run in a Docker container. A build step can do anything that can be done from a container irrespective of the environment. To perform your tasks, you can either use the supported build steps provided by Cloud Build or write your own build steps.  

Supported Build Steps → https://cloud.google.com/build/docs/deploying-builds/deploy-cloud-run  
Write your own build steps → https://cloud.google.com/build/docs/configuring-builds/use-community-and-custom-builders  

Cluster nodes Auto-upgrading https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-upgrades   
Cluster nodes Auto-repair https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-repair  

A Kubernetes cluster is composed of nodes, which are a unit of hardware resources. Nodes in GKE are implemented as VMs in Compute Engine. Each node has pods. Pods are resource management units. A pod is how Kubernetes controls and manages resources needed by applications and how it executes code. Pods also give the system fine-grain control over scaling. Each pod hosts, manages, and runs one or more containers. The containers in a pod
share networking and storage. So typically, there is one container per pod, unless the containers hold closely related applications. For example, a second container might contain the logging system for the application in the first container. A pod can be moved from one node to another without reconfiguring or rebuilding anything. Each cluster has a control plane node that determines what happens on the cluster. There are usually at least three of them for availability. And they can be located across zones. A Kubernetes job makes changes to the cluster. For example a pod YAML file provides the information to start up and run a pod on a node. If for some reason a pod stops running or a node is lost, the pod will not automatically be replaced. The Deployment YAML tells Kubernetes how many pods you want running. So the Kubernetes deployment is what keeps a number of pods running. The Deployment YAML also defines a Replica Set, which is how many copies of a container you want running. The Kubernetes scheduler determines on which node and in which pod the replica containers are to be run.

Types of clusters (Standard vs Autopilot, Regional vs Zonal) https://cloud.google.com/kubernetes-engine/docs/concepts/types-of-cluster   
AutoPilot https://cloud.google.com/kubernetes-engine/docs/concepts/autopilot-overview  
Overview of deploying workloads https://cloud.google.com/kubernetes-engine/docs/how-to/deploying-workloads-overview  
Services https://cloud.google.com/kubernetes-engine/docs/concepts/service  
Another overview: https://kubernetes.io/docs/concepts/services-networking/service/  
Exposing applications using services (includes add, edit and remove): https://cloud.google.com/kubernetes-engine/docs/how-to/exposing-apps  
GKE Services https://cloud.google.com/kubernetes-engine/docs/concepts/service  
About node pools https://cloud.google.com/kubernetes-engine/docs/concepts/node-pools  
Configuring multidimensional Pod autoscaling https://cloud.google.com/kubernetes-engine/docs/how-to/multidimensional-pod-autoscaling
Recommendations for planning, architecting, deploying, scaling, and operating large workloads on Google Kubernetes Engine (GKE) clusters https://cloud.google.com/kubernetes-engine/docs/best-practices/scalability  
For more details on Requests and Limits, see: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/  
Cluster nodes scaling https://cloud.google.com/kubernetes-engine/docs/concepts/cluster-autoscaler  
Using node auto-provisioning https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-provisioning  
Enabling node auto-provisioning: https://cloud.google.com/kubernetes-engine/docs/how-to/node-auto-provisioning#enable  
Horizontal pod scaling https://cloud.google.com/kubernetes-engine/docs/concepts/horizontalpodautoscaler  
Custom and external metrics for Horizontal autoscaling workloads: https://cloud.google.com/kubernetes-engine/docs/concepts/custom-and-external-metrics  
Vertical pod scaling https://cloud.google.com/kubernetes-engine/docs/concepts/verticalpodautoscaler  
Youtube - Autoscaling with GKE https://www.youtube.com/watch?v=7naCIxIaV1M  


Pods are the smallest unit of deployment. A pod can be comprised of one or more containers, but typically it is one pod per container.  
Clusters are a collection of instances the containers can run on. Each instance is a node in a cluster.  
Replica sets are used to create multiple instances of a pod. The replica sets can guarantee the desired number is always running and only healthy pods are used.  
Kubernetes can leverage cloud load balancers to distribute traffic to multiple pods.  
The load balancer is run as a network service.  
To ensure the proper performance of your application, you can configure autoscalers to add and remove pods.  
Deployments are configurations that define service resources.  

App Engine is a fully managed, serverless application platform supporting the building and deploying of applications. Applications can be scaled seamlessly from zero upward without having to worry about managing the underlying infrastructure. App Engine was designed for microservices. For configuration, each Google Cloud project can contain one App Engine application, and an application has one or more services. Each service can have one or more versions, and each version has one or more instances. App Engine supports traffic splitting so it makes switching between versions and strategies such as canary testing or A/B testing simple. The diagram on the right shows the high-level organization of a Google Cloud project with two services, and each service has two versions. These services are independently deployable and versioned.  

Your Hybrid Cloud Strategy https://cloud.google.com/files/kubernetes-your-hybrid-cloud-strategy.pdf  

## Day 10
#### 28 APR 2023  



Identity Aware Proxy https://cloud.google.com/iap/docs/concepts-overview  
Identity-Aware Proxy https://cloud.google.com/iap  
IAP overview: https://cloud.google.com/iap/docs/concepts-overview  
IAP Enabling external identities: https://cloud.google.com/iap/docs/enable-external-identities    
Cloud IAP enables context-aware access to VMs via SSH and RDP without bastion hosts   https://cloud.google.com/blog/products/identity-security/cloud-iap-enables-context-aware-access-to-vms-via-ssh-and-rdp-without-bastion-hosts/   
Youtube: Centralize access to your organization’s websites with Identity Aware Proxy (IAP) https://www.youtube.com/watch?v=xM9-FSU5MoY  

Apigee https://docs.apigee.com/   
Apigee Youtube: https://www.youtube.com/watch?v=58smxQu3P5k  
Apigee Demo videos https://cloud.google.com/apigee/demo-ty  
Cloud Endpoints https://cloud.google.com/endpoints  
Encryption at rest in Google Cloud https://cloud.google.com/docs/security/encryption/default-encryption  
Encryption in Transit in Google Cloud https://cloud.google.com/docs/security/encryption-in-transit  
Customer-managed encryption keys (CMEK) https://cloud.google.com/kms/docs/cmek  
Customer-Supplied Encryption Keys https://cloud.google.com/docs/security/encryption/customer-supplied-encryption-keys  
Secret Manager https://cloud.google.com/secret-manager  
Managing Cloud Run secrets securely https://www.youtube.com/watch?v=JIE89dneaGo  
Cloud Data Loss Prevention https://cloud.google.com/dlp  
Improving security, compliance, and governance with cloud-based DLP data discovery https://cloud.google.com/blog/products/identity-security/modern-dlp-for-cloud-data-discovery  
VPC Service Controls https://cloud.google.com/vpc-service-controls/docs/overview  
Private Google Access for on-premises hosts https://cloud.google.com/vpc/docs/private-google-access-hybrid  
Centralize access to your organization’s websites with Identity Aware Proxy (IAP) Youtube link on slide: https://www.youtube.com/watch?v=xM9-FSU5MoY  
Getting started with BeyondCorp: A deeper look into IAP Youtube: https://www.youtube.com/watch?v=goAWiQGRefw&t=341s  
BeyondCorp Enterprise https://cloud.google.com/beyondcorp-enterprise  
Cloud IAP for on prem apps overview https://cloud.google.com/iap/docs/cloud-iap-for-on-prem-apps-overview  
Cloud IAP enables context-aware access to VMs via SSH and RDP without bastion hosts https://cloud.google.com/blog/products/identity-security/cloud-iap-enables-context-aware-access-to-vms-via-ssh-and-rdp-without-bastion-hosts/  
Identity-Aware Proxy for TCP Forwarding: https://cloud.google.com/iap/docs/tcp-forwarding-overview  
Using IAP for TCP forwarding https://cloud.google.com/iap/docs/using-tcp-forwarding  
How Kitabisa re-structured its fundraising platform to drive "kindness at scale" on Google Cloud https://cloud.google.com/blog/products/application-development/how-kitabisa-uses-google-cloud-gke-cloud-sql-and-proxysql/  
More about Kitabisa https://kitabisa.com/  
Deployment Manager is Google Cloud’s IaC tool https://cloud.google.com/deployment-manager/docs  

Terraform https://www.terraform.io/  
Once the template is built, use terraform commands to make changes  
- terraform init : get plugins if needed  
- terraform plan : checks for errors in the terraform file  
- terraform apply : applies the file and creates the resources  
- terraform delete : deletes the resources  

Cloud Foundation Toolkit https://cloud.google.com/foundation-toolkit   
Google Cloud Security, Privacy and Compliance https://cloud.google.com/security  
Compliance Resource Center https://cloud.google.com/security/compliance/  

Shared responsibility
PCI (Payment Card Industry) compliance https://cloud.google.com/solutions/pci-dss-compliance-in-gcp  
HIPAA compliance (US) https://cloud.google.com/security/compliance/hipaa-compliance  
GDPR compliance https://cloud.google.com/security/gdpr  

Security Command Center https://cloud.google.com/security-command-center
Security Command Center conceptual overview: https://cloud.google.com/security-command-center/docs/concepts-security-commandcenter-overview
OWASP Top 10 https://www.hacksplaining.com/owasp  
NIST 800-53: Definition and Tips for Compliance: https://www.varonis.com/blog/nist-800-53  
Container Threat Detection https://cloud.google.com/blog/products/identity-security/container-threat-detection-is-ga  
Tier Information https://cloud.google.com/security-command-center/docs/concepts-security-commandcenter-overview

Recommended Videos
Six Part Video Series - Security Command Center (June 2020 - Dec 2020) https://www.youtube.com/watch?v=Q-fzz2P6omQ&list=PLIivdWyY5sqKd-Cu1HZ7v5RiYE8gVsM7P&index=2
Security Talks: Improve your security posture with the Security Command Center (Nov 18, 2020) https://www.youtube.com/watch?v=4nelxX_1erk&t=20s  

Google Cloud infrastructure reliability guide https://cloud.google.com/architecture/infra-reliability-guide  
Everything you need to know about architecting reliable infrastructure for Google Cloud workloads https://cloud.google.com/blog/products/infrastructure-modernization/design-reliable-infrastructure-for-workloads-in-google-cloud  
Google Cloud Architecture Framework: Reliability https://cloud.google.com/architecture/framework/reliability  
Design for scale and high availability https://cloud.google.com/architecture/framework/reliability/design-scale-high-availability  
Product reliability guides https://cloud.google.com/architecture/framework/reliability/product-guides  
Design for high availability https://cloud.google.com/architecture/scalable-and-resilient-apps#physically_distribute_resources  

Patterns for scalable and resilient apps: https://cloud.google.com/architecture/scalable-and-resilient-apps  
Autoscaling Cloud Spanner: https://cloud.google.com/architecture/autoscaling-cloud-spanner  
Bigtable scaling: https://cloud.google.com/bigtable/docs/scaling  
Memorystore scaling: https://cloud.google.com/memorystore/docs/redis/scaling-instances#  
Disaster Recovery Planning Guide https://cloud.google.com/architecture/dr-scenarios-planning-guide  
Cloud Monitoring https://cloud.google.com/monitoring  
Custom metrics https://cloud.google.com/monitoring/custom-metrics  
OpenCensus: https://opencensus.io/  
Uptime checks https://cloud.google.com/monitoring/uptime-checks  
Cloud Logging pricing for Cloud Admins: How to approach it & save cost https://cloud.google.com/blog/topics/cost-management/how-to-approach-cloud-logging-pricing-for-cloud-admins  
Cloud Logging https://cloud.google.com/logging/docs  
Log data compliance: https://services.google.com/fh/files/misc/whitepaper_data_governance_logs_how_to.pdf  
Configuring log sinks to export logs to external systems (e.g., on-premises or BigQuery) https://cloud.google.com/logging/docs/routing/overview  
Scenarios for exporting Cloud Logging data - Splunk https://cloud.google.com/architecture/exporting-stackdriver-logging-for-splunk  
View logs in sink destinations: https://cloud.google.com/logging/docs/export/using_exported_logs  
Log sinks: https://cloud.google.com/logging/docs/export/configure_export_v2  
Cloud Trace https://cloud.google.com/trace  
Viewing trace details: https://cloud.google.com/trace/docs/viewing-details  
Cloud Profiler https://cloud.google.com/profiler/docs  
Cloud Error Reporting https://cloud.google.com/error-reporting  

## Day 11
#### 3 MAY 2023  

Disaster recovery planning guide https://cloud.google.com/architecture/dr-scenarios-planning-guide  
Refactoring a monolith into microservices https://cloud.google.com/architecture/microservices-architecture-refactoring-monoliths   
Infrastructure as a code (IaaC) https://cloud.google.com/recommender/docs/tutorial-iac  
Active Assist https://cloud.google.com/recommender/docs/whatis-activeassist  
Cloud Foundation Toolkit https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit  
Security Command Center https://cloud.google.com/security-command-center  
News : https://thenewstack.io/paris-is-drowning-gcps-region-failure-in-age-of-operational-resilience/  
Multi container apps https://docs.docker.com/get-started/07_multi_container/  
How multi-container works https://medium.com/bb-tutorials-and-thoughts/understanding-multi-container-pods-12f5780f3956  
Cloud Trace filters https://cloud.google.com/trace/docs/trace-filters  

## Day 12
#### 5 MAY 2023  
Exam Details shared and practiced few test questions.    
