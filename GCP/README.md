# #60DaystoGCP-ACE

<p align="center">
  <img src="/Content/rainbow.png">
</p>

** DISCLAIMER: This is not 40 days continuous journey to certification as initially advised. But since I had 45 hours workweek and weekend classes as well while taking the exam, I had to start the countdown somewhere so that I take the certification ASAP. However, if you've time, I would suggest 45 days of self study around GCP Engineer prep material on Google Cloud portal (including labs) + 10 days of exam prep questions prep from Udemy and voila, CERTIFIED!  

However, if you're on a Beast Mode, 30 days of self study + 10 days of questionnaire, but for how many exams can we be on a beast mode, hence, I enjoyed food too, instead of following a strict diet during exam time. :D         

Images Source: https://github.com/priyankavergadia, https://cloud.google.com/blog/topics/developers-practitioners/network-application-security-google-cloud/    
Starter Link: https://betterprogramming.pub/gcp-and-aws-networking-concepts-and-services-ef8264cfa5a8  
   
- [ ] Feb 1 2023 > Went through the GCP Engineer starter introduction on YouTube https://www.youtube.com/watch?v=RbIbS0YMFs4&t=1395&ab_channel=GoogleCloud    
- [ ] Feb 13 2023 > Went through the IAM & GCP marketplace to understand LAMP deployment in the GCP Engineer coursework https://cloud.google.com/marketplace/docs/  
- [ ] Feb 14 2023 > Went through LAB today: Getting Started with VPC Networking and Google Compute Engine  
- [ ] Feb 16 2023 > Today, I decided to go through the playlist on Cracking the Google Cloud career https://bit.ly/3xsYrRp  
- [ ] Feb 18 2023 > Found this GitHub cheatsheet link on GCP https://github.com/priyankavergadia/google-cloud-4-words#the-google-cloud-developers-cheat-sheet   
- [ ] Feb 19 2023 > Revisited few basics of GCP on Coursera, pay attention to **pricing model**  
- [ ] Feb 23 2023 > Going through Essential Cloud Infrastructure: Foundation  
- [ ] Feb 26 2023 > Going through Sample GCP questions today on https://www.whizlabs.com/blog/gcp-associate-cloud-engineer-questions/  
- [ ] Feb 27 2023 > GCP Partner training started in my office. For the next 15 days, I will be religiously pursuing that material  
- [ ] Feb 28 2023 > Cheatsheet and cloud comparison https://cloud.google.com/free/docs/aws-azure-gcp-service-comparison, https://googlecloudcheatsheet.withgoogle.com/ 
- [ ] 1 MAR 2023 > Working with the flash cards for the D-Day revision, back to school methods @35 :D.   
        1. **Introduction to VPC & Subnets** https://cloud.google.com/vpc/docs/overview  
        2. **IAM basics** https://cloud.google.com/iam/docs/understanding-roles, https://cloud.google.com/iam/docs/permissions-reference     
        3. **IP & CIDR**  
        4. **Regions & Zones (World)** https://cloud.google.com/compute/docs/regions-zones  
        5. **VPC Peering** https://cloud.google.com/vpc/docs/vpc-peering, https://cloud.google.com/vpc/docs/quota  
        6. **Load Balancing & Auto Scaling** https://cloud.google.com/load-balancing/docs/load-balancing-overview , https://cloud.google.com/load-balancing/docs  
        7. **VPC Network** https://cloud.google.com/vpc/docs/vpc   
        8. **VPC Flow Logs** https://cloud.google.com/vpc/docs/flow-logs   
        9. **Health Checks** https://cloud.google.com/load-balancing/docs/health-check-concepts  
        10. **Billing** When billing costs exceed a percentage of your budget, based on the rules you set, alert notifications are sent to billing administrators and billing account users. GCP will not stop services and will not delete anything https://cloud.google.com/billing/docs/concepts, https://cloud.google.com/billing/docs/how-to/budgets  
        11. **Resource Manager** https://cloud.google.com/resource-manager  
        12. **Restricting Resources** (Org) https://cloud.google.com/resource-manager/docs/organization-policy/defining-locations  
        13. **Cloud Identity** https://cloud.google.com/identity, https://cloud.google.com/identity/docs/overview  
        14. **gcloud configurations** https://cloud.google.com/sdk/docs/configurations  
        15. **Authorize the gcloud CLI** https://cloud.google.com/sdk/docs/authorizing  
        16. **Bring Your Own IP (BYOIP)** https://cloud.google.com/vpc/docs/bring-your-own-ip  
        
Internal IPs = private   
External IPs = public   

<br/> 

| Command |	Description |
| --- | --- |
| gcloud init |	Authorizes access and performs other common setup steps |
| gcloud auth login |	Authorizes access only |

<br/>

| Name | Title | Permissions |
| --- | --- | --- |
| **roles/viewer** | Viewer	| Permissions for read-only actions that do not affect state, such as viewing (but not modifying) existing resources or data |
| **roles/editor** | Editor | All viewer permissions, plus permissions for actions that modify state, such as changing existing resources |
| **roles/owner** |	Owner |	All Editor permissions and permissions for the following actions: Manage roles and permissions for a project and all resources within the project & Set up billing for a project |

<br/>
<p>
   <img src="/Content/choose-lb.svg">
</p>

- [ ] 2 MAR 2023 > GCP Partner training update: Came across a new feature Security Hardening https://cloud.google.com/managed-microsoft-ad/docs/hardening   
        1. **VP Networks lab**  https://partner.cloudskillsboost.google/course_templates/479?catalog_rank={%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue}&search_id=22588454  
        2. **Firewall (Ingress & Egress) i.e. incoming & outgoing** https://cloud.google.com/vpc/docs/about-firewalls, https://cloud.google.com/vpc/docs/firewalls <br/><br/> 
            &emsp;&emsp;&emsp;&emsp;a. **Hierarchical firewall policy** In this policy, you create and enforce a consistent firewall policy across your organization. You can assign hierarchical firewall policies to the organization as a whole or to individual folders. These policies contain rules that can explicitly deny or allow connections. In addition, hierarchical firewall policy rules can delegate evaluation to lower-level policies or VPC network firewall rules with a goto_next action. Lower-level rules cannot override a rule from a higher place in the resource hierarchy. This lets organization-wide admins manage critical firewall rules in one place. https://cloud.google.com/vpc/docs/firewall-policies-examples  
            &emsp;&emsp;&emsp;&emsp;b. **Global firewall policy** Global network firewall policies enable you to batch update all firewall rules by grouping them into a single policy object https://cloud.google.com/vpc/docs/use-network-firewall-policies   
            &emsp;&emsp;&emsp;&emsp;c. **Regional firewall policy** Regional network firewall policies let you create and enforce a consistent firewall policy across all subnetworks within a region in your VPC network. These policies contain rules that can explicitly deny or allow connections, or go to the next level of the hierarchy https://cloud.google.com/vpc/docs/use-regional-firewall-policies   <br/><br/>
        4. **Routes** https://cloud.google.com/vpc/docs/routes  
        5. **Compute Engine & Options** https://cloud.google.com/compute, Create a persistent disk from a data source  https://cloud.google.com/compute/docs/disks/create-disk-from-source     
        6. **Cluster Security & Security Hardening** https://cloud.google.com/kubernetes-engine/docs/concepts/security-overview, https://cloud.google.com/kubernetes-engine/docs/how-to/hardening-your-cluster     
        7. **NAT Gateway & Bastion Host** Cloud NAT enables you to provision your application instances without public IP addresses while also allowing them to access the internet for updates, patching, config management, and more in a controlled and efficient manner. https://cloud.google.com/nat/docs/overview  
        8. **Cloud Storage** : https://cloud.google.com/products/storage, https://cloud.google.com/storage/docs/access-control/making-data-public    
        9. **Other Recommendation** :
        Recommendation for ACE and PCA  
        <br/><br/>
            &emsp;&emsp;&emsp;&emsp;a. **Basic of Networking**   https://www.youtube.com/watch?v=EuSFNggRCH8&t=1306s   
            &emsp;&emsp;&emsp;&emsp;b. https://www.computernetworkingnotes.com/ccna-study-guide/subnetting-tricks-subnetting-made-easy-with-examples.html  
            &emsp;&emsp;&emsp;&emsp;c. **Basic of Linux Server** https://www.elithecomputerguy.com/linux-new/  
            &emsp;&emsp;&emsp;&emsp;d. **Basic Database** https://www.elithecomputerguy.com/mysql-introduction-2019/  
            &emsp;&emsp;&emsp;&emsp;e. **Basic of Storage** https://www.youtube.com/watch?v=1Dqsi2M2tgM  
            &emsp;&emsp;&emsp;&emsp;f. **Basic Virtualization** https://www.youtube.com/watch?v=FZR0rG3HKIk   
            &emsp;&emsp;&emsp;&emsp;g. **Basic of Scripting (Powershell, JSON scripting , Python scripting)** https://www.youtube.com/watch?v=kpuAr6hbRuk  
            &emsp;&emsp;&emsp;&emsp;h. **Basic of Windows Server** https://www.elithecomputerguy.com/windows-server-2012/   
        10. **Dynamic Routing** https://cloud.google.com/network-connectivity/docs/router/how-to/configuring-routing-mode  
        11. **Cloud Router** Google Cloud Router enables you to dynamically exchange routes between your Virtual Private Cloud (VPC) and on-premises networks by using Border Gateway Protocol (BGP). The Cloud Router automatically learns new subnets in your VPC network and announces them to your on-premises network. https://cloud.google.com/network-connectivity/docs/router/concepts/overview   
        12. **BGP Peering** https://cloud.google.com/network-connectivity/docs/router/how-to/configuring-bgp  
        13. **VPN Tunnel** https://cloud.google.com/network-connectivity/docs/vpn/how-to/adding-a-tunnel  
        14. **Cloud VPN** https://cloud.google.com/network-connectivity/docs/vpn/concepts/overview  
        15. **Cloud Interconnect** https://cloud.google.com/network-connectivity/docs/interconnect/concepts/overview   
        16. **Stackdriver Logging** https://cloud.google.com/migrate/compute-engine/docs/4.8/how-to/monitoring/using-stackdriver-monitoring   
        17. **Cloud CDN** leverages Google’s globally distributed edge points of presence to accelerate content delivery for websites and applications served out of Google Compute Engine and Google Cloud Storage. Cloud CDN lowers network latency, offloads origins, and reduces serving costs. https://cloud.google.com/cdn/docs/overview    
        18. **Cloud Run** is a managed compute platform that automatically scales your stateless containers. https://cloud.google.com/run, https://cloud.google.com/run/docs/apis    
        19. **API Gateway** https://cloud.google.com/api-gateway  
        20. **Stackdriver or Google Cloud Operations Suite** https://cloud.google.com/products/operations, https://cloud.google.com/stackdriver/docs  
        21. **Cloud Functions** https://cloud.google.com/functions/docs  
        22. **API Engine** https://cloud.google.com/appengine/docs/the-appengine-environments  
        23. **What is a Cloud Run** https://cloud.google.com/run/docs/overview/what-is-cloud-run  
        24. **ACL** https://cloud.google.com/storage/docs/access-control/lists  
        <br/>
        <br/>
        
| Service | Description (Migration) |
| ------ | ------ |
| **Google Cloud Router** | Google Cloud Router enables you to dynamically exchange routes between your Virtual Private Cloud (VPC) and on-premises networks by using Border Gateway Protocol (BGP). The Cloud Router automatically learns new subnets in your VPC network and announces them to your on-premises network. |
| **Cloud CDN** | Cloud CDN leverages Google’s globally distributed edge points of presence to accelerate content delivery for websites and applications served out of Google Compute Engine and Google Cloud Storage. Cloud CDN lowers network latency, offloads origins, and reduces serving costs. |
| **Cloud NAT** | Cloud NAT enables you to provision your application instances without public IP addresses while also allowing them to access the internet for updates, patching, config management, and more in a controlled and efficient manner. |
| **Cloud Run** | Cloud Run is a managed compute platform that automatically scales your stateless containers. | 

<br/>  
<p>
  <img src="/Content/hfw3-2.svg" width="500" align="top"/>
  <img width="100"/>
  <img src="/Content/firewall.jpg" width="400" align="top"/>
</p>
  
- [ ] 3 MAR 2023 >  In Depth understanding of the cloud setup for the basic application     
        1. **Storage & Databases (Object, File, Relational, Non-realtional, Warehouse)** : https://cloud.google.com/products/storage, https://cloud.google.com/products/databases  
        2. **Shared Responsibility Model**: https://cloud.google.com/architecture/framework/security/shared-responsibility-shared-fate  
        3. **Storage Types** : Storage -> Nearline (1 Month) -> Coldline (3 Month) -> Archive (1 Year) (arranged as per frequecy usage/ data retrieval)  
        4. **Storage Options** : Region, Dual-region, Multi-region https://cloud.google.com/storage/docs/storage-classes, https://cloud.google.com/storage/docs/locations    
        5. **Pricing** : https://cloud.google.com/storage/pricing  
        6. **Object Lifecycle Management** : If you want to delete the data but want to contain the snapshot of the data for few days before deleting it. https://cloud.google.com/storage/docs/lifecycle  
        7. **Object Immutability** : https://cloud.google.com/storage/docs/objects  
        8. **Object Versioning** : Maintaining multiple version on the object or maintaining the history https://cloud.google.com/storage/docs/object-versioning  
        9. **Delete Policy** : https://cloud.google.com/iam/docs/reference/rest/v2beta/policies/delete   
        10. **Filestore** : https://cloud.google.com/filestore  
        11. **Netapp** : https://cloud.google.com/architecture/partners/netapp-cloud-volumes  
        12. **Azure-AWS-GCP Comparison** : https://cloud.google.com/free/docs/aws-azure-gcp-service-comparison  
        13. **ACID Properties** : https://www.bmc.com/blogs/acid-atomic-consistent-isolated-durable/  
        14. **GCP Services** : https://cloud.google.com/terms/services  
        15. **Scaling Application** : https://cloud.google.com/community/tutorials/horizontally-scale-mysql-database-backend-with-google-cloud-sql-and-proxysql, https://cloud.google.com/architecture/elastically-scaling-your-mysql-environment  
        16. **Create Read Replicas** : https://cloud.google.com/sql/docs/postgres/replication/create-replica, https://cloud.google.com/sql/docs/mysql/replication   
        17. **Transfer Cloud Storage to Cloud Storage use cases** https://cloud.google.com/storage-transfer/docs/cloud-storage-to-cloud-storage  
<br/>

| Storage Options | Description |
| --- | --- |
| **Google Storage Standard (None)** | Google Storage Standard is not a cheap option for storing archive data. There are other options to store archive data cheaper |
| **Google Storage Nearline (30 days)** | Nearline is to plan archive data accessed **at most once a month** |
| **Google Storage Coldline (90 days)** | Google Cloud Storage Coldline is a low-cost, highly durable storage service for storing infrequently accessed data. Coldline Storage is ideal for data you plan to read or modify on average **once a quarter or less.** |
| **Google Archive (365 days)** | Google Cloud Storage Coldline is a low-cost, highly durable storage service for storing infrequently accessed data. Coldline Storage is ideal for data you plan to read or modify on average **once a quarter or less.** |
| **BigQuery** | BigQuery does not have cheaper cost for storing data than Nearline for the first 90 days until it’s moved to long-term storage | 
<br/>

<p>
   <img src="/Content/Storage-to-Use.jpeg">
</p>

- [ ] 6 MAR 2023 > Storage Options (BigQuery -> Dataflow -> Dataprep -> Dataproc -> Result)   
        1. **Bigquery** : https://cloud.google.com/bigquery, https://cloud.google.com/bigquery/docs/batch-loading-data    
        2. **Cloud Spanner** : https://cloud.google.com/spanner  
        3. **Firestore** : https://cloud.google.com/firestore  
        4. **Cloud Bigtable** : https://cloud.google.com/bigtable  
        5. **Memorystore** : https://cloud.google.com/memorystore  
        6. **Security** : https://cloud.google.com/security, https://cloud.google.com/docs/security/encryption-in-transit    
        7. **Shared Responsibility Model** : https://cloud.google.com/architecture/framework/security/shared-responsibility-shared-fate  
        8. **Performance & IOPS** : https://cloud.google.com/compute/docs/disks/performance  
        9. **Encryption Options** : https://cloud.google.com/docs/security/encryption/default-encryption    
        10. **Cloud Key Management** : https://cloud.google.com/security-key-management  
        11. **Cloud EKM** : https://cloud.google.com/cloud-provider-access-management/key-access-justifications/docs/overview   
        12. **Compliance** : https://cloud.google.com/security/compliance  ..look PCI DSS standard   
        13. **GDPR** : https://cloud.google.com/privacy/gdpr  
        14. **Private Google Access** : https://cloud.google.com/vpc/docs/private-google-access   
        15. **Pricing (dual region vs single region)** : https://cloud.google.com/products/calculator , https://cloud.google.com/storage/docs/locations, https://cloud.google.com/bigquery/pricing    
        16. In BigQuery, by limiting the number of columns to required ones you will be able to reduce the amount of data processed by BigQuery thus saving cost. Grouping query result does not help in reducing cost. It just groups result depending on the column specified. Then, Composite key will not help in reducing cost. This is only used to create unique records in a table. Also, JOINS are used when you are querying data from more than one table, this will not help.  

<br/>

| Service | Description |
| --- | --- |
| **BigTable** | BigTable is a managed NoSQL DB service designed for handling and processing large amounts of data |  
| **BigQuery** | BigQuery is a relational database service, hence cannot be used to store non-relational data. BigQuery is also a regional service and cannot be scaled horizontally |   
| **Datastore** | Datastore is NoSQL managed DB service but the amount of data we are looking at is quite big for Datastore to efficiently process. Datastore also supports ACID transactions but is not horizontally scalable and is a NoSQL database |  
| **Google Cloud Storage** | GCS is only used for storing files. It does not support relational or non-relational data |
| **CloudSQL** | CloudSQL provides database migration service as well as MySQL managed DB service. CloudSQL supports ACID transactions but supports only vertical scaling. CloudSQL only supports MySQL, SQL Server and Postgres. Therefore, it does not fit our requirement. For Oracle and DB2, the only option is to install both of them on a VM |  
| **Cloud Spanner** | Cloud Spanner is a global SQL database service that can scale across the globe horizontally and even supports ACID transactions | 
| **Cloud Dataproc** | Cloud Dataproc is a fast, easy-to-use, fully managed cloud service for running Apache Spark and Apache Hadoop clusters in a simpler, more cost-efficient way |
| **Cloud Dataflow** | Cloud Dataflow is a fully-managed service for transforming and enriching data in stream (real time) and batch (historical) modes with equal reliability and expressiveness |
| **Cloud Composer** | Cloud Composer is a fully managed workflow orchestration service that empowers you to author, schedule, and monitor pipelines that span across clouds and on-premises data centers. It is built on the popular Apache Airflow open source project |

<br/>

| Role | Description |
| --- | --- |
| **Cloud SQL Editor** | SQL Editor allows users to Manage specific instances. No ability to see or modify permissions, nor modify users or SSL certs. No ability to import data or restore from a backup, nor clone, delete, or promote instances |
| **Cloud SQL Admin** | Full control for all Cloud SQL resources |
| **Cloud SQL Viewer** | Read-only access to all Cloud SQL resources |
| **Cloud SQL Client** | Connectivity access to Cloud SQL instances from App Engine and the Cloud SQL Proxy. Not required for accessing an instance using IP addresses | 

<br/><br/>
<p>
   <img src="/Content/Which-GCP-Database.jpg"/>
</p>
<p>
   <img src="/Content/big_table.png"/>
</p>


- [ ] 7 MAR 2023 > Security Contd.  Deployments -> Rolling, Blue green, canary  
        1. **Security** : https://cloud.google.com/security-command-center, https://partner.cloudskillsboost.google/course_templates/88?catalog_rank={%22rank%22%3A2%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue}&search_id=22645730   
        2. **DDoS Attack** : https://cloud.google.com/armor, https://cloud.google.com/blog/products/identity-security/how-google-cloud-blocked-largest-layer-7-ddos-attack-at-46-million-rps  
        3. **GCP WAF** : https://cloud.google.com/blog/products/identity-security/new-waf-capabilities-in-cloud-armor  
        4. **Cloud Operations Suite (Refer Log Sink)** : https://cloud.google.com/products/operations, https://cloud.google.com/logging/docs/export/configure_export_v2, https://services.google.com/fh/files/misc/whitepaper_data_governance_logs_how_to.pdf      
        5. **Cloud Monitoring** : https://cloud.google.com/monitoring/docs/monitoring-overview   
        6. **Cloud Trace** : https://cloud.google.com/trace   
        7. **Error Reporting** : https://cloud.google.com/error-reporting  
        8. **Cloud logs** : https://cloud.google.com/logging/docs/view/logs-explorer-interface, https://cloud.google.com/debugger/docs  
        9. **Cloud Profiler** : https://cloud.google.com/profiler/docs/about-profiler , https://cloud.google.com/profiler/docs    
        10. **Deployments** : https://www.techtarget.com/searchitoperations/answer/When-to-use-canary-vs-blue-green-vs-rolling-deployment  
        11. **Cost Management** : https://cloud.google.com/cost-management  
        12. **Best Practices** : https://cloud.google.com/blog/topics/cost-management/best-practices-for-optimizing-your-cloud-costs  
        13. **Pricing Calculator**: https://cloud.google.com/products/calculator  
        14. **Resource Hierarchy** : https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy  
        15. **Book on Google Cloud Security Foundations (120 pages)** : https://services.google.com/fh/files/misc/google-cloud-security-foundations-guide.pdf  
        16. **Financial Governance on the Cloud** : https://cloud.google.com/files/guide-to-financial-governance.pdf  
        17. **Troubleshooting** : https://cloud.google.com/storage/docs/troubleshooting, https://cloud.google.com/compute/docs/troubleshooting/troubleshooting-rdp   
<br/>


| Service | Description |
| --- | --- |
| **Stackdriver Trace** | Stackdriver Trace is a distributed tracing system that collects latency data from your applications and displays it in the Google Cloud Platform Console. You can track how requests propagate through your application and receive detailed near real-time performance insights |
| **Profiler** | Profiler helps you continuously monitor CPU and heap profiling |
| **Stackdriver Monitoring** | Stackdriver Monitoring provides visibility into the performance, uptime, and overall health of cloud-powered applications |
| **Activity Logs** | Activity logs record API activities such as launching of instance, creating firewall, attaching it to instance, creating bucket, etc. Activity logs records each and every activity performed by a user or resources like creating, deleting a VM |
| **Flow Logs** | Flow logs capture each and every packet flowing within your network. It will record details like source IP, destination IP, source port, destination port, timestamp, etc. |

<br/>
<p>
   <img src="/Content/network_n_security.jpg"/>
</p>
<p>
   <img src="/Content/cloud_armor.jpg"/>
</p>

- [ ] 9 MAR 2023 > CI/CD and DevOps Automation    
        1. **DevOps & SRE** : https://sre.google/, https://cloud.google.com/blog/products/devops-sre/dora-2022-accelerate-state-of-devops-report-now-out, https://thenewstack.io/google-reveals-the-secrets-of-devops/  
        2. **Continuous Integration** : https://cloud.google.com/solutions/continuous-integration  
        3. **GKE** : https://cloud.google.com/kubernetes-engine, https://cloud.google.com/kubernetes-engine/docs/concepts/kubernetes-engine-overview    
        4. **App Engine** : Each project has 1 app engine, cannot have more than that https://cloud.google.com/appengine Google App Engine is only used to deploy applications.  
        5. **Application Architecture: Monolithic vs SOA vs Microservices** : https://www.coforge.com/blog/application-architecture-monolithic-vs-soa-vs-microservices  
        6. **MIGs** : https://cloud.google.com/compute/docs/instance-groups#managed_instance_groups, https://cloud.google.com/compute/docs/instance-groups/creating-groups-of-managed-instances   
        7. **OSI Model (Extra)** : https://www.elithecomputerguy.com/2010/07/osi-model-demystified/  

<p>
   <img src="/Content/api_management.jpg"/>
</p>
<p>
   <img src="/Content/api_security.png"/>
</p>

- [ ] 10 MAR 2023 > Lab Today  
        1. **Networking lab**  
        2. **VM Instance lab**   
        3. **MIG Lab, predictive autoscaling**   
        4. **Cloud balancing** : https://cloudsolutions.academy/solution/what-is-anycast-ip-address-and-how-does-google-cloud-load-balancer-works/  
        5. **Resource hierarchy** : https://cloud.google.com/iam/docs/overview, https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy  
        6. **External HTTP(S) load balancer overview** : https://cloud.google.com/load-balancing/docs/https  
        

**Resource hierarchy**  
Google Cloud resources are organized hierarchically:

&emsp; &emsp;- The organization is the root node in the hierarchy.  
&emsp; &emsp;- Folders are children of the organization.  
&emsp; &emsp;- Projects are children of the organization, or of a folder.  
&emsp; &emsp;- Resources for each service are descendants of projects.  
&emsp; &emsp;- Each resource has exactly one parent. For more information, see the Resource Manager resource hierarchy.  

The following diagram is an example of a Google Cloud resource hierarchy.

<p align="center">
   <img src="/Content/policy-inheritance.svg"/>
</p>

**Link with Google Workspace or Cloud Identity accounts**  

The Google Workspace or Cloud Identity account represents a company and is a prerequisite to have access to the organization resource. In the Google Cloud context, it provides identity management, recovery mechanism, ownership and lifecycle management. The picture below shows the link between the Google Workspace account, Cloud Identity, and the Google Cloud resource hierarchy.

<p align="center">
   <img src="/Content/cloud-hierarchy-workspace.svg"/>
</p>

**IAM policy inheritance**  

Google Cloud offers IAM, which lets you assign granular access to specific Google Cloud resources and prevents unwanted access to other resources. IAM lets you control who (users) has what access (roles) to which resources by setting IAM policies on the resources.

You can set an IAM policy at the organization level, the folder level, the project level, or (in some cases) the resource level. Resources inherit the policies of the parent resource. If you set a policy at the organization level, it is inherited by all its child folder and project resources, and if you set a policy at the project level, it is inherited by all its child resources.

The effective policy for a resource is the union of the policy set on the resource and the policy inherited from its ancestors. This inheritance is transitive. In other words, resources inherit policies from the project, which inherit policies from the organization resource. Therefore, the organization-level policies also apply at the resource level.

<p align="center">
   <img src="/Content/cloud-hierarchy.svg"/>
</p>


- [ ] 13 MAR 2023 > Hybrid networking, Pub/Sub, Cloud Functions, Cloud Run  
        1. **Serverless** : https://cloud.google.com/serverless  
        2. **YouTube Library on Pub/Sub** :   
        3. **Where to run my stuff** : https://cloud.google.com/blog/topics/developers-practitioners/where-should-i-run-my-stuff-choosing-google-cloud-compute-option         4. **Cloud Functions** :  https://cloud.google.com/functions  
        4. **Cloud Functions Lab** : https://partner.cloudskillsboost.google/focuses/11542?catalog_rank={%22rank%22%3A13%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue}&parent=catalog&search_id=16956267  
        5. **Cloud Functions vs Cloud Run** : Both are serverless and auto scaled but when you binary depencies, and program is written in Rust, use Cloud run  
        6. **Cloud Run** : When you have a container and don't want to use GKE, cloud run is used. https://cloud.google.com/run, https://cloud.google.com/run/docs, https://knative.dev/docs/, https://www.virtasant.com/blog/stateful-vs-stateless-architecture-why-stateless-won  

<p align="center">
   <img src="/Content/gke-architecture.svg"/>
</p>
  
 
- [ ] 14 MAR 2023 > Containers and Kubernetes. Also, today is the last day of my GCP ACE training, hopefully, I'll take exam in coming weeks...  
        1. **Hypervisor vs OS**  
        2. **Containers vs Docker** : https://blog.purestorage.com/purely-informational/containerd-vs-docker-whats-the-difference/  
        3. **CI/CD** : https://cloud.google.com/solutions/continuous-integration, https://cloud.google.com/docs/ci-cd  
        4. **Artifact Registry** : https://cloud.google.com/artifact-registry, https://cloud.google.com/artifact-registry/docs  
        5. **Kubernetes Cheatsheet** : https://kubernetes.io/docs/reference/kubectl/cheatsheet/  
        6. **gcloud cheatsheet** : https://cloud.google.com/sdk/docs/cheatsheet, https://cloud.google.com/static/sdk/docs/images/gcloud-cheat-sheet.pdf, https://googlecloudcheatsheet.withgoogle.com/  
        7. **GKE Documentation** : https://cloud.google.com/kubernetes-engine/docs/concepts/kubernetes-engine-overview   
        8. **Services** : https://cloud.google.com/kubernetes-engine/docs/concepts/service    
        9. **Another overview** : https://kubernetes.io/docs/concepts/services-networking/service/    
        10. **Exposing applications using services (includes add, edit and remove)** : https://cloud.google.com/kubernetes-engine/docs/how-to/exposing-apps    
        11. **Deployments** : https://kubernetes.io/docs/concepts/workloads/controllers/deployment/   
        12. **Suggested Lab: Running a MongoDB Database in Kubernetes with StatefulSets**: https://partner.cloudskillsboost.google/focuses/14656?parent=catalog  
        13. **Lab 2** : https://partner.cloudskillsboost.google/course_templates/2   
        14. **GKE Reference Doc** : https://storage.googleapis.com/cloud-training/T-KUBGKE-I/v1.7/Student%20PDFs/%5BT-KUBGKE-B%5D%20%20M2_%20Introduction%20to%20Containers%20and%20Kubernetes_ILT%20v1.7.pdf   
        15. **Kubernetes Architecture** : https://storage.googleapis.com/cloud-training/T-KUBGKE-I/v1.7/Student%20PDFs/%5BT-KUBGKE-B%5D%20M3_%20Kubernetes%20Architecture_ILT%20v1.7.pdf   
        16. **Kubernetes Workloads** : https://storage.googleapis.com/cloud-training/T-KUBGKE-I/v1.7/Student%20PDFs/%5BT-KUBGKE-B%5D%20%20M4_%20Introduction%20to%20Kubernetes%20Workloads%20v1.7.pdf   
        17. **Configuring multidimensional Pod autoscaling** : https://cloud.google.com/kubernetes-engine/docs/how-to/multidimensional-pod-autoscaling  
        18. **Transfer Appliance** : https://cloud.google.com/transfer-appliance/docs/4.0/overview  
        19. **Where to run my stuff** : https://cloud.google.com/blog/topics/developers-practitioners/where-should-i-run-my-stuff-choosing-google-cloud-compute-option  
<br/>

| Engine | Description |
| --- | --- |
| **App Engine** | A fully managed serverless platform for complete web applications. App Engine handles the networking, application scaling, and database scaling. You write a web application in one of the supported languages, deploy to App Engine, and it handles scaling, updating versions, and so on |
| **Compute Engine** | Virtual machines. You reserve a configuration of CPU, memory, disk, and GPUs, and decide what OS and additional software to run |
| **Cloud Run** | A fully managed serverless platform that runs individual containers. You give code or a container to Cloud Run, and it hosts and auto scales as needed to respond to web and other events |
| **Cloud Functions**| Event-driven serverless functions. You write individual function code and Cloud Functions calls your function when events happen (for example, HTTP, Pub/Sub, and Cloud Storage changes, among others) |
| **GKE** | Managed Kubernetes clusters. Kubernetes is an open-source system for automating deployment, scaling, and management of containerized applications. You create a cluster and configure which containers to run; Kubernetes keeps them running and manages scaling, updates and connectivity |

<br/>
<p>
  <img src="/Content/Engine.jpg"/>
</p>
<br/>
  
 
- [ ] 14 MAR 2023 > ************************************************************SELF STUDY STARTS NOW**************************************************************
- [ ] 20 MAR 2023 > Test day next month, wish me luck!:crossed_fingers: Example pipeline below  

### GKE learning pipeline
<p align="center">
   <img src="/Content/gco-cloud-network.png" width="700px" alt="https://cloudplatform.googleblog.com/2018/06/Behind-the-scenes-with-the-Dragon-Ball-Legends-GCP-backend.html">
</p>

### Machine learning pipeline
<p>
  <img src="/Content/BigQuery.webp"/>
</p>

First 3 things  
.  
https://cloud.google.com/docs/get-started  
https://cloud.google.com/communities  
https://www.googlecloudcommunity.com/gc/Google-Cloud/ct-p/google-cloud  
Get your hands dirty https://console.cloud.google.com/  

**A. Google recommended Labwork on Fundatmentals**  
- [X] CLoud Storage and Cloud SQL  
- [X] Cloud Marketplace  
- [X] VPC networking and Compute Engine  
- [X] Getting started with Cloud Storage and Cloud SQL  
- [X] Getting started with GKE  
- [X] Hello Cloud Run  
- [X] Automating the deployment of Infrastructure using Terraform   
- [X] Logging and Monitoring in the cloud  
  
**B. Google recommended Labwork on Infrastructure Foundation**  
- [X] Google cloud console and cloud shell  
- [X] Infrastructure Preview   
- [X] VPC networking -> create VPC, VM instances, firewall, subnets ( on UI and **shell**)  
- [X] Implement Private Google Access and Cloud NAT  -> VPC N/Ws with firewall, VM instances, tunnel through iap, and bucket, nat gateway and nat router, stackdriver logging with transalation & errors
- [X] Creating virtual machines ->  
- [X] Working with virtual machines ->   
  
**C. Google recommended Labwork on Infrstructure Core Services**
- [X] IAM -> Policy on the folder or service  
- [X] Cloud Storage -> bucket creation and accessing on private and public addresses   
- [X] Cloud SQL -> Connecting to MySQL on GCP for CDN such as Wordpress and working on the blog  
- [X] Billing Data and BigQuery -> We can see all data using BigQuery  
- [X] Resource Monitoring -> for spikes on server, create dashboards  
- [X] Error Reporting and Debugging -> create alerts on six different mediums for notifications   
  
**D. Google recommended Labwork on Scaling and Automation**  
- [X] Cloud HA VPN  
- [X] Autoscaling and Loadbalancing -> Create firewall rule, nat gateway, vm instances, start apache server, create mig for europe and us with health check, configure load balancer, perform stress test on IPv4    
- [X] Configuring Load balancer -> firewall rule, cloud NAT, two VM instances, two MIGs, TCP Load Balancing for internal load balncing with front end and back end configurations against MIGs and health check    
- [X] Automating the infrastructure of networks using Terraform  
- 
  **Further Reading** 
  1. https://www.cloudskillsboost.google/focuses/2794?parent=catalog  
  2. https://cloud.google.com/sre, https://cloud.google.com/blog/products/devops-sre/  
  3. https://cloud.google.com/blog/products/devops-sre/devsecops-and-cicd-using-google-cloud-built-in-services  
  4. https://cloud.google.com/blog/  
 
**E. Google recommended Labwork on GKE**  
- [X] Working with Cloud Build  
- [X] Deploying to Google Kuberenetes Engine  


**Next Steps**

1. Labwork  
2. Commands -> gsutil, gscloud, curl, terraform, apache, apt-get and so on  
3. Configurations  

**Extra : From APIGEE Training**

1. https://docs.apigee.com/hybrid/logging  
2. https://docs.apigee.com/hybrid/ts-cassandra  
3. https://docs.apigee.com/hybrid/ts-message-processor  
4. https://kubernetes.io/docs/tasks/debug-application-cluster  

**Prep material**:
1. Preparing for Google Cloud Certification: Cloud Engineer Professional Certificate (Coursera)  
2. Preparing for Google Cloud Certification: Cloud Engineer Professional Certificate (Google Cloud SkillBoost)   
3. https://research.google/teams/network-systems/, https://research.google/teams/cloud-networking/
4. https://docs.gcp.databricks.com/data-governance/best-practices.html, Use case on Unity https://docs.gcp.databricks.com/data-governance/unity-catalog/get-started.html  
5. https://cloud.google.com/network-intelligence-center/docs/network-topology/concepts/overview
6. https://cloud.google.com/architecture/hybrid-and-multi-cloud-network-topologies 
        
