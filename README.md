# Setup kubernetes
https://www.digitalocean.com/community/tutorials/how-to-create-a-kubernetes-1-10-cluster-using-kubeadm-on-ubuntu-16-04
- kubelet
- kubeadm
- kubectl


## Network
https://medium.com/google-cloud/kubernetes-nodeport-vs-loadbalancer-vs-ingress-when-should-i-use-what-922f010849e0
### ClusterIP
default k8s service
```
kubectl proxy --port=8080
http://localhost:8080/api/v1/proxy/namespaces/<NAMESPACE>/services/<SERVICE-NAME>:<PORT-NAME>/
```

### NodePort
direct traffic to services
- once service per port
- only port 30000-32767

### LoadBalancer

### Ingress
Ingress Controller: Google Cloud Load Balance, Nginx, Contour, Isio, Kong
