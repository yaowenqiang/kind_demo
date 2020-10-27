> curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.9.0/kind-linux-amd64
> chmod +x ./kind
> mv ./kind /usr/local/bin/kind
> kind create cluster
> kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0/aio/deploy/recommended.yaml

> # access  api remotely
> kubectl proxy
> ssh -L 8001:127.0.0.1:8001 root@10.4.42.51 

> create a user
> https://github.com/kubernetes/dashboard/blob/master/docs/user/access-control/creating-sample-user.md

> http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/ 

> https://kube-2019-01.container.training/#2

> kubectl cluster-info --context kind-kind

