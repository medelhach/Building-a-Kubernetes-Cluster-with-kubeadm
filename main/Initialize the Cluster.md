* Initialize the Kubernetes cluster on the Control-Plane-VM using kubeadm .

(Note: This is only performed on the Control-Plane-VM):
```
sudo kubeadm init --pod-network-cidr 192.168.0.0/16 --kubernetes-version 1.24.0
```
* Set kubectl access:
```
mkdir -p $HOME/.kube
sudo cp -i /etc/kubernetes/admin.conf $HOME/.kube/config
sudo chown $(id -u):$(id -g) $HOME/.kube/config
```
* Test access to cluster:
```
kubectl get nodes
```
