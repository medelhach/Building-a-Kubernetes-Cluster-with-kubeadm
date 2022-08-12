* In the Control-Plane-VM, create the token and copy the kubeadm join command :
```
kubeadm token create --print-join-command
```
* In both worker-vm , paste the kubeadm join command to join the cluster. Use sudo to run it as root:
```
sudo kubeadm join ...
```
* In the Control-Plane-VM, view cluster status (Note: You may have to wait a few moments to allow all nodes to become ready):
```
kubectl get nodes
```
