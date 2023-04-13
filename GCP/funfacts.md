Both Ingress and Egress -> The priority of a firewall rule can range from 0 to 65535. The lower the number, the higher the priority. The default priority when you create a new rule is 1000.
Refer https://cloud.google.com/vpc/docs/firewalls 
<br/>
| Instance machine type | Maximum number of stateful connections |
| --- | --- |
| Shared-core machine types | 130,000 |
| Instances with 1–8 vCPUs | 130,000 connections per vCPU |
| Instances with more than 8 vCPUs | 1,040,000 (130,000×8) connections total |
<br/>

