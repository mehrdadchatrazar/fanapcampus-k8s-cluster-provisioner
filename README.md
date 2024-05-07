# Fanapcampus K8S Cluster Provisioner

This Ansible project automates the deployment of a Kubernetes cluster with a single master node and a scalable number of worker nodes. It leverages CRI-O as the container runtime and Calico for networking.


## Requirements

### Operating System:
Master and Worker Nodes: Ubuntu 22.04 LTS (or compatible)

### Software:
- Ansible
- Python
- SSH access to the target nodes
- A user named ubuntu on your nodes

## Usage
1. Edit inventory file (host.yaml): Replace the placeholder hostnames with the actual hostnames or IP addresses of your master and worker nodes.
2. Run the playbook:
    ```
    ansible-playbook -i host.yml site.yml
    ```
This will execute the Ansible playbook and provision the Kubernetes cluster.

## Notes

- This project is provided as-is for educational and demonstration purposes. You might need to adapt it to your specific environment and security requirements.
- Refer to the Kubernetes documentation (https://kubernetes.io/docs/setup/) for more in-depth instructions and best practices.