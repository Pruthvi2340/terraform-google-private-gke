# This module creates private GKE cluster with custom VPC and CIDR ranges
# This module with comes with argo-cd installation

# Release 1.0.0
Description added with the initial requirements for CD infrastructure creation

```
project_id = ""
name = "retail-demo-app"
region = "us-central1"
node_machine_type = "e2-standard-4"
node_count = 2
vpc_primary_cidr = "10.0.0.0/18"
k8s_pods_secondary_cidr = "10.48.0.0/14"
k8s_service_secondary_cidr ="10.52.0.0/20"
```

# Release 1.0.4

Description: master authorized network to 0.0.0.0/0

# Release 1.0.5

Description: added permissions to Kubernetes Service account

# Release 1.0.6

Description: deletion protection set to false

# Release 1.0.7

Description: argocd upgraded to 2.3.0

# Release 1.0.8

Description: static ip for ingress and DNS

# Release 1.0.9

Description: Http load balancing enabled

# Release 1.0.10

Description: Firewall network tags to allow health checks for ingress backend