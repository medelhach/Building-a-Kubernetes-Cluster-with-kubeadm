After creating the three VMs . we specify one to be the Control-Plane-VM and the two ather will be worker-vm1 and worker-vm2 . 

# Install Packages

* Log into the control Control-Plane-VM
* Create configuration file for containerd:
```
cat <<EOF | sudo tee /etc/modules-load.d/containerd.conf
overlay
br_netfilter
EOF
```
