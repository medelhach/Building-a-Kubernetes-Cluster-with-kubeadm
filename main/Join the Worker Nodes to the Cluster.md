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

and the Final result is 

```
azureuser@vm1kub:~$ kubectl get nodes
NAME         STATUS   ROLES           AGE   VERSION
nodevm2kub   Ready    <none>          87s   v1.24.0
nodevm3kub   Ready    <none>          99s   v1.24.0
vm1kub       Ready    control-plane   47m   v1.24.0


```
