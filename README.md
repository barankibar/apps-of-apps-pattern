# Overview
This repository demonstrates the "App of Apps" pattern in ArgoCD. The structure allows for managing multiple Kubernetes applications through a single root application, streamlining the deployment and management process.

## Repository Structure
-   **root.yaml**: The parent application manifest that references all child applications.
-   **app-manifests/**: Directory containing ArgoCD Application definitions for each child application.
-   **applications/**: Directory containing Kubernetes manifests (Deployments, Services, Ingresses) for individual applications.


## Directory Structure
```yaml
├── applications/
│ ├── app1/ 
│ │ ├── deployment.yaml 
│ └── app2/ 
│ ├── deployment.yaml 
│ ├── service.yaml 
│ └── ingress.yaml 
├── app-manifests/
│ ├── app1.yaml
│ └── app2.yaml
├── README.md 
└── root.yaml
```
