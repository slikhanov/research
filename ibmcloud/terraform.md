# IBM Cloud Terraform Provider

## Things I wish I knew

1. Creating `ibm_resource_group` in the same state as for example `ibm_kubernetes_cluster` is not a great idea.
   `ibm_kubernetes_cluster` creates multiple resources and all of them are attached to given resource. When you
   decide to destroy state it will fail, because cluster will get destroyed, but automatically created worker nodes will not.
   As result `ibm_resource_group` destruction will also fail.
