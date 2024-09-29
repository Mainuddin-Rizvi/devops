Here are essential Kubernetes, kubectl, and Minikube commands in a (link unavailable) structure:

Kubernetes Commands

Cluster Management

- kubectl get nodes - List cluster nodes
- kubectl describe node <node-name> - Describe a node
- kubectl get pods - List pods
- kubectl get deployments - List deployments
- kubectl get services - List services
- kubectl get persistentvolumes - List persistent volumes
- kubectl get storageclasses - List storage classes

Pod Management

- kubectl run <pod-name> --image=<image-name> - Run a pod
- kubectl get pod <pod-name> - Get pod details
- kubectl describe pod <pod-name> - Describe a pod
- kubectl logs <pod-name> - View pod logs
- kubectl exec <pod-name> -- <command> - Execute command in pod
- kubectl delete pod <pod-name> - Delete a pod

Deployment Management

- kubectl create deployment <deployment-name> --image=<image-name> - Create deployment
- kubectl get deployments - List deployments
- kubectl describe deployment <deployment-name> - Describe deployment
- kubectl rollout status deployment <deployment-name> - Check rollout status
- kubectl rollout undo deployment <deployment-name> - Undo rollout
- kubectl scale deployment <deployment-name> --replicas=<num> - Scale deployment

Service Management

- kubectl expose deployment <deployment-name> --type=<service-type> - Expose deployment as service
- kubectl get services - List services
- kubectl describe service <service-name> - Describe service

Persistent Volume Management

- kubectl create pv <pv-name> --capacity=<size> - Create persistent volume
- kubectl get pv - List persistent volumes
- kubectl describe pv <pv-name> - Describe persistent volume

ConfigMap and Secret Management

- kubectl create configmap <cm-name> --from-literal=<key>=<value> - Create config map
- kubectl get configmaps - List config maps
- kubectl describe configmap <cm-name> - Describe config map
- kubectl create secret generic <secret-name> --from-literal=<key>=<value> - Create secret

Networking

- kubectl get ingresses - List ingresses
- kubectl describe ingress <ingress-name> - Describe ingress

Security

- kubectl get clusterroles - List cluster roles
- kubectl describe clusterrole <clusterrole-name> - Describe cluster role
- kubectl get rolebindings - List role bindings
- kubectl describe rolebinding <rolebinding-name> - Describe role binding

Backup and Restore

- kubectl get backups - List backups (Velero)
- kubectl describe backup <backup-name> - Describe backup (Velero)
- kubectl restore <backup-name> - Restore from backup (Velero)

kubectl Commands

kubectl get

- kubectl get <resource-type> <resource-name>
- kubectl get <resource-type> -n <namespace>

kubectl describe

- kubectl describe <resource-type> <resource-name>
- kubectl describe <resource-type> -n <namespace>

kubectl create

- kubectl create -f <manifest-file>.yaml
- kubectl create <resource-type> <resource-name> --image=<image-name>

kubectl apply

- kubectl apply -f <manifest-file>.yaml

kubectl delete

- kubectl delete <resource-type> <resource-name>
- kubectl delete -f <manifest-file>.yaml

Minikube Commands

Minikube Start/Stop

- minikube start - Start Minikube
- minikube stop - Stop Minikube

Minikube Cluster Management

- minikube status - Check Minikube status
- minikube delete - Delete Minikube cluster

Minikube Dashboard

- minikube dashboard - Open Minikube dashboard

Minikube Addons

- minikube addons list - List available addons
- minikube addons enable <addon-name> - Enable addon
- minikube addons disable <addon-name> - Disable addon

kubeadm Commands

kubeadm Init

- kubeadm init - Initialize Kubernetes cluster

kubeadm Join

- kubeadm join <master-node-ip>:<port> - Join node to cluster

kubeadm Upgrade

- kubeadm upgrade plan - Check upgrade plan
- kubeadm upgrade apply - Apply upgrade

kubeadm Reset

- kubeadm reset - Reset Kubernetes cluster

Note: This
