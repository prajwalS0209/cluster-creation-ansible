# Kubernetes Cluster Network Configuration

## Slave Configuration

- **NodePort Ports:** 30000 - 32767/TCP
- **Kubelet API:** 10248 - 10260/TCP
- **Weave Net Port (UDP):** 6784
- **Weave Net Port (TCP):** 6783
- **SSH Connection:** 22/SSH

## Master Configuration

- **Weave Net Port (UDP):** 6784
- **Weave Net Port (TCP):** 6783
- **NodePorts:** 30000 - 32767/TCP
- **etcd Server:** 2379 - 2380/TCP
- **Kubernetes API Server:** 6443/TCP
- **Kubernetes Tools:** 10248 - 10260/TCP
- **SSH Connection:** 22/SSH


![alt text](https://github.com/prajwalS0209/cluster-creation-ansible/blob/main/Screenshot%202024-03-27%20at%201.14.51%20PM.png)