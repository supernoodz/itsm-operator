Kubernetes Ansible Operator which creates and updates a Service Now record for Namespace CRUD operations.

## Implementation

# Clone

$ git clone https://github.com/supernoodz/itsm-operator

$ cd itsm-operator

# Modify

$ Edit deploy/operator.yaml to include your Service Now instance, credentials and table.

# Deploy

$ kubectl create -f deploy/role_binding.yaml

$ kubectl create -f deploy/role.yaml

$ kubectl create -f deploy/service_account.yaml

$ kubectl create -f deploy/operator.yaml

# Monitor

$ kubectl get pods -w

$ kubectl logs POD -f operator

# Remove

$ kubectl delete -f deploy/role_binding.yaml

$ kubectl delete -f deploy/role.yaml

$ kubectl delete -f deploy/service_account.yaml

$ kubectl delete -f deploy/operator.yaml
