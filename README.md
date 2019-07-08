# itsm-operator

# Clone
$ git clone https://github.com/supernoodz/itsm-operator
$ cd itsm-operator

# Deploy
$ kubectl create -f deploy/role_binding.yaml
$ kubectl create -f deploy/role.yaml
$ kubectl create -f deploy/service_account.yaml
$ kubectl create -f deploy/operator.yaml

# Monitor
$ kubectl get pods -w
$ kubectl get logs <pod> -f operator

# Remove
$ kubectl delete -f deploy/role_binding.yaml
$ kubectl delete -f deploy/role.yaml
$ kubectl delete -f deploy/service_account.yaml
$ kubectl delete -f deploy/operator.yaml
