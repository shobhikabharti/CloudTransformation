Example here -> https://cloud.google.com/sdk/gcloud/reference/compute/instances/describe, https://cloud.google.com/sdk/gcloud/reference/compute/instances/create, https://kubernetes.io/docs/reference/kubectl/cheatsheet/  

**gcloud format**

gcloud + release level (optional) + component + entity + operation + positional args + flags  
For example: gcloud + compute + instances + create + example-instance-1 + --zone=us-central1-a  

**Release level**
Release Level refers to the command’s release status.  

Example: alpha for alpha commands, beta for beta commands, no release level needed for GA commands.  

**Component**  
Component refers to the different Google Cloud services.  

Example: compute for Compute Engine, app for App Engine, etc.  

**Entity**  
Entity refers to the plural form of an element or collection of elements under a component.  

Example: disks, firewalls, images, instances, regions, zones for compute  

**Operation**  
Operation refers to the imperative verb form of the operation to be performed on the entity.  

Example: Common operations are describe, list, create/update, delete/clear, import, export, copy, remove, add, reset, restart, restore, run, and deploy.  

**Positional args**  
Positional args refer to the required, order-specific arguments needed to execute the command.  

Example: <INSTANCE_NAMES> is the required positional argument for gcloud compute instances create.  

**Flags**  
Flags refer to the additional arguments, --flag-name(=value), passed in to the command after positional args.  

Example: --machine-type=<MACHINE_TYPE> and --preemptible are optional flags for gcloud compute instances create.  

**Global flags**  
Some flags are available throughout the gcloud CLI experience, like:  
--help: For when in doubt; display detailed help for a command.  
--project: If using a project other than the current one.  
--quiet: Disabling interactive prompting (and applying default values for inputs).  
--verbosity: Can set verbosity levels at debug, info, warning, error, critical, and none.  
--version: Display gcloud version information.  
--format: Set output format as config, csv, default, diff, disable, flattened, get, json, list, multi, none, object, table, text, value, or yaml.  

**Authentication and Configuration**  
gcloud init: Initialize the gcloud configuration and setup a new configuration or switch to an existing one.  
gcloud auth login: Authorize Google Cloud access for the gcloud CLI with Google Cloud user credentials and set the current account as active.  
gcloud auth activate-service-account: Authorize Google Cloud access similar to gcloud auth login but with service account credentials.  
gcloud auth application-default: Manage your Application Default Credentials (ADC) for Cloud Client Libraries.  
gcloud auth list: List all credentialed accounts.  
gcloud auth print-access-token: Display the current account's access token.   
gcloud auth revoke: Remove access credentials for an account.  

**IAM**

gcloud iam list-grantable-roles: List IAM grantable roles for a resource.  
gcloud iam roles create: Create a custom role for a project or org.  
gcloud iam service-accounts create: Create a service account for a project.  
gcloud iam service-accounts add-iam-policy-binding: Add an IAM policy binding to a service account.  
gcloud iam service-accounts set-iam-policy-binding: Replace existing IAM policy binding.  
gcloud iam service-accounts keys list: List a service account's keys.  

**Manage Projects**

gcloud projects describe: Display metadata for a project (including its ID).
gcloud projects add-iam-policy-binding: Add an IAM policy binding to a specified project.

**Virtual Machine & Compute Engine**   
gcloud compute instances create: Create a new Compute Engine instance.  
gcloud compute instances list: List all the Compute Engine instances in your project.  
gcloud compute ssh: SSH into a Compute Engine instance.  
gcloud compute disks create: Create a new disk for a Compute Engine instance.  
gcloud compute firewall-rules create: Create a new firewall rule for Compute Engine instances.   
gcloud compute zones list: List Compute Engine zones.  
gcloud compute instances create: Create a VM instance.  
gcloud compute instances describe: Display a VM instance's details.  
gcloud compute instances list: List all VM instances in a project.  
gcloud compute disks snapshot: Create snapshot of persistent disks.  
gcloud compute snapshots describe: Display a snapshot's details.  
gcloud compute snapshots delete: Delete a snapshot.  
gcloud compute ssh: Connect to a VM instance by using SSH.  
gcloud compute project-info describe --project PROJECT_ID :  see what your default region and zone settings.  
-> https://cloud.google.com/compute/docs/gcloud-compute#set_default_zone_and_region_in_your_local_client  
Health Check  
gcloud compute firewall-rules create default-allow-health-check \
--direction=INGRESS --priority=1000 --network=default \
--action=ALLOW --rules=tcp:80 \
--source-ranges=130.211.0.0/22,35.191.0.0/16 \
--target-tags=allow-health-check

**Cloud Storage**  
gcloud storage buckets create: Create a new Cloud Storage bucket.  
gcloud storage buckets list: List all the Cloud Storage buckets in your project.  
gsutil cp: Copy files to and from Cloud Storage buckets.  
gsutil rsync: Synchronize files between local directories and Cloud Storage buckets.  

**Docker & Kubernetes Engine**  
gcloud container clusters create: Create a new Kubernetes Engine cluster.  
gcloud container clusters get-credentials: Get authentication credentials for a Kubernetes Engine cluster.  
kubectl: Interact with a Kubernetes Engine cluster using the Kubernetes command-line tool.  
gcloud auth configure-docker: Register the gcloud CLI as a Docker credential helper.  
gcloud container clusters create: Create a cluster to run GKE containers.  
gcloud container clusters list: List clusters for running GKE containers.  
gcloud container clusters get-credentials: Update kubeconfig to get kubectl to use a GKE cluster.  
gcloud container images list-tags: List tag and digest metadata for a container image.  

**Serverless & App Engine**  
gcloud app deploy: Deploy an App Engine application.  
gcloud app versions list: List all the versions of your App Engine application.  
gcloud app services list: List all the services in your App Engine application.  
gcloud app deploy: Deploy your app's code and configuration to the App Engine server.  
gcloud app versions list: List all versions of all services deployed to the App Engine server.  
gcloud app browse: Open the current app in a web browser.  
gcloud app create: Create an App Engine app within your current project.  
gcloud app logs read: Display the latest App Engine app logs.  

**Cloud SQL**  
gcloud sql instances create: Create a new Cloud SQL instance.  
gcloud sql instances list: List all the Cloud SQL instances in your project.  
gcloud sql databases create: Create a new database in a Cloud SQL instance.  

**Get going with the gcloud CLI.**

gcloud init: Initialize, authorize, and configure the gcloud CLI.  
gcloud version: Display version and installed components.  
gcloud components install: Install specific components.  
gcloud components update: Update your gcloud CLI to the latest version.  
gcloud config set project: Set a default Google Cloud project to work on.  
gcloud info: Display current gcloud CLI environment details.  

**Personalization**

gcloud config set: Define a property (like compute/zone) for the current configuration.  
gcloud config get: Fetch the value of a gcloud CLI property.  
gcloud config list: Display all the properties for the current configuration.  
gcloud config configurations create: Create a new named configuration.  
gcloud config configurations list: Display a list of all available configurations.  
gcloud config configurations activate: Switch to an existing named configuration.  

**Miscellaneous**
gcloud kms decrypt: Decrypt ciphertext (to a plaintext file) using a Cloud Key Management Service key.
gcloud logging logs list: List your project's logs.
gcloud sql backups describe: Display info about a Cloud SQL instance backup.
gcloud sql export sql: Export data from a Cloud SQL instance to a SQL file.

**Help**

gcloud help: Search the gcloud CLI reference documents for specific terms.
gcloud feedback: Provide feedback to the gcloud CLI team.
gcloud topic: Supplementary help material for non-command topics like accessibility, filtering, and formatting.

**Authentication and Configuration**  
gsutil config: Configure gsutil.  
gsutil help: Get help with gsutil commands.  
gsutil version: Check the version of gsutil you are running.  
gsutil ls: List all Cloud Storage buckets.  
gcloud init: Initialize the gcloud configuration and setup a new configuration or switch to an existing one.  
gcloud auth login: Log in to your Google Cloud Platform account and authorize the gsutil tool to access your resources.  

**Buckets**  
gsutil mb: Create a new Cloud Storage bucket.  
gsutil rb: Remove a Cloud Storage bucket.  
gsutil acl: Modify access control lists for a bucket or object.  
gsutil defacl: Modify default object access control lists for a bucket.  
gsutil label: Modify labels for a bucket.  
gsutil lifecycle: Configure lifecycle management policies for a bucket.  
gsutil retention: Configure retention policies for a bucket.  
gsutil web: Configure website settings for a bucket.  

**Objects**  
gsutil cp: Copy files to and from Cloud Storage buckets.  
gsutil mv: Move files between Cloud Storage buckets or folders.  
gsutil rm: Delete one or more objects from a bucket.  
gsutil ls: List objects in a bucket.  
gsutil du: Show disk usage information for a bucket or object.  
gsutil cat: Display the contents of a Cloud Storage object.  
gsutil setmeta: Set or remove metadata on a bucket or object.  
gsutil compose: Concatenate multiple objects into a single object.  
gsutil hash: Compute and display a hash of an object's data.  

**Accessing Data**  
gsutil cp: Copy files to and from Cloud Storage buckets.  
gsutil rsync: Synchronize files between local directories and Cloud Storage buckets.  
gsutil streaming: Stream data into or out of Cloud Storage buckets.  

**Data Transfer**  
gsutil cp: Copy files to and from Cloud Storage buckets.  
gsutil rsync: Synchronize files between local directories and Cloud Storage buckets.  
gsutil transfer: Schedule and manage transfers between Cloud Storage buckets.  

**Basics**  
curl [URL]: Send a GET request to a URL and display the response in the terminal.  
curl -I [URL]: Send a HEAD request to a URL and display the response headers in the terminal.  

**Request Methods**  
curl [URL]: Send a Get request to a URL.  
curl -X POST [URL]: Send a POST request to a URL.  
curl -X PUT [URL]: Send a PUT request to a URL.  
curl -X DELETE [URL]: Send a DELETE request to a URL.  

**Request Data**  
curl -d [data] [URL]: Send data in the request body using the POST method.  
curl -F [data] [URL]: Send data as a multipart/form-data using the POST method.  
curl -H [header] [URL]: Set a custom header in the request.  

**Authentication**  
curl -u [username:password] [URL]: Authenticate with basic auth.  
curl --cert [path_to_cert] --key [path_to_key] [URL]: Authenticate with a client certificate.  

**Output**  
curl -o [filename] [URL]: Save the response body to a file.  
curl -O [URL]: Save the response body to a file with the same name as the URL.  
curl -v [URL]: Display verbose output, including request and response headers.  

**Advanced**  
curl -H "Content-Type: application/json" -d '{"key": "value"}' [URL]: Send a JSON payload in the request body.  
curl -G -d 'param1=value1&param2=value2' [URL]: Send a GET request with query parameters.  
curl --resolve [host:port:ip_address] [URL]: Resolve a host to a specific IP address.  


Reference here:  
https://cloud.google.com/sdk/docs/cheatsheet,   
https://cloud.google.com/sdk/gcloud/reference/compute,  
https://mishnit.github.io/cheatsheet-gcp-A4.pdf,  
https://cloud.in28minutes.com/gcp-certification-cloud-storage,  
https://linuxopsys.com/topics/linux-commands-cheat-sheet        
