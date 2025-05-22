## Kubernetes Architectures

Kubernetes is designed with a master-worker architecture. The main components are:

- **Control Plane (Master Node):**
    - `kube-apiserver`: Serves the Kubernetes API.
    - `etcd`: Stores cluster data.
    - `kube-scheduler`: Assigns workloads to nodes.
    - `kube-controller-manager`: Runs controllers to regulate cluster state.
    - `cloud-controller-manager`: Integrates with cloud providers.

- **Worker Nodes:**
    - `kubelet`: Ensures containers are running.
    - `kube-proxy`: Handles networking and load balancing.
    - `Container runtime`: Runs containers (e.g., Docker, containerd).

### High-Level Architecture Diagram

```
[ Control Plane ]
            |
[ Worker Nodes ] -- [ Pods/Containers ]
```

---

## Common Kubernetes Interview Questions

1. **What is Kubernetes and why is it used?**
2. **Explain the Kubernetes architecture.**
3. **What are Pods, Deployments, and Services?**
4. **How does Kubernetes handle scaling and self-healing?**
5. **What is etcd and what role does it play?**
6. **How do you perform rolling updates in Kubernetes?**
7. **What is a Namespace in Kubernetes?**
8. **How does Kubernetes networking work?**
9. **What are ConfigMaps and Secrets?**
10. **How do you secure a Kubernetes cluster?**