# Rancher Managed Cluster

## Prerequisites

In order to deploy the environment at least 3 masters and 2 workers VMs will be needed.  
Recommended resources:
 - Masters: 2CPUs and 2Gi (min) 
 - Workers: 4CPUs and 4Gi (min) 

This playbook has been tested just in RHEL 8.5 VMs with the mentioned resources with satisfactory results.

The VMs must have the hostname and static IPs configured and if possible the ssh key added. 

A DNS server is helpful in order to guarantee the servers' visibility. For this example a VM running containerized pihole and configured as dns server in the VMs was enough.

***
Before the plan execution we need a token generated in the rancher manager UI in order to authorize the api calls. The token var: 'cluster_api_key'


## License

This project is under the Apache License 2.0 - take a look to the LICENSE file for more details.
