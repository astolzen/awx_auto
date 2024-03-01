# AWX automated rollout and configuration
#### v 0.1 230301

This set of playbooks will roll out an AWX Insance on Openshift or Microshift (Other Kubernetes Distros possible, change "Route"-COde to "Ingress")

### Requirements:
 - Kubernetes Node or Cluster, Auth via kubeconfig file
 - AWX-Operator installed on Kuberentes Setup

### Customization:
  - Add Credentials to secrets.yml. It's recommended to encrypt it with vault, after keys and passwords are inserted
  - Add your AWX confiuration as code into vars.yml

### further customization
 - add additional variables into vars and 02_awx_config as needed. Exmples: Workflow templates or additionale Template fields like Instance Groups
 - add options for dynamic Inventories

