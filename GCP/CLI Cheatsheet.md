**Authentication and Configuration**  
gcloud init: Initialize the gcloud configuration and setup a new configuration or switch to an existing one.  
gcloud auth login: Log in to your Google Cloud Platform account and authorize the gcloud tool to access your resources.  

**Compute Engine**   
gcloud compute instances create: Create a new Compute Engine instance.  
gcloud compute instances list: List all the Compute Engine instances in your project.  
gcloud compute ssh: SSH into a Compute Engine instance.  
gcloud compute disks create: Create a new disk for a Compute Engine instance.  
gcloud compute firewall-rules create: Create a new firewall rule for Compute Engine instances.  

**Cloud Storage**  
gcloud storage buckets create: Create a new Cloud Storage bucket.  
gcloud storage buckets list: List all the Cloud Storage buckets in your project.  
gsutil cp: Copy files to and from Cloud Storage buckets.  
gsutil rsync: Synchronize files between local directories and Cloud Storage buckets.  

**Kubernetes Engine**  
gcloud container clusters create: Create a new Kubernetes Engine cluster.  
gcloud container clusters get-credentials: Get authentication credentials for a Kubernetes Engine cluster.  
kubectl: Interact with a Kubernetes Engine cluster using the Kubernetes command-line tool.  

**App Engine**  
gcloud app deploy: Deploy an App Engine application.  
gcloud app versions list: List all the versions of your App Engine application.  
gcloud app services list: List all the services in your App Engine application.  

**Cloud SQL**  
gcloud sql instances create: Create a new Cloud SQL instance.  
gcloud sql instances list: List all the Cloud SQL instances in your project.  
gcloud sql databases create: Create a new database in a Cloud SQL instance.  


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
