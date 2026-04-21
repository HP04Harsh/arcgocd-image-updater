🚀 ArgoCD Masterclass Demos
===========================

This repository is a hands-on laboratory for mastering **GitOps with ArgoCD**. The core manifests are inspired by the **TrainWithShubham (TWS)** and **Amitabh DevOps** masterclasses, which I am actively adapting and updating to deepen my understanding of Kubernetes automation.

📂 Project Structure
--------------------

This repo is organized into modules that cover the full spectrum of ArgoCD capabilities:

*   **App of Apps Pattern**: Manage multiple applications (Apache, Nginx, Online Shop) through a single root "parent" application.
    
*   **ApplicationSets**: Templates for scaling deployments across multiple clusters or namespaces automatically.
    
*   **CLI Approach**: Examples for managing, syncing, and troubleshooting apps via the argocd command line.
    
*   **Declarative Approach**: Pure YAML-based definitions for managing "Applications as Code."
    
*   **Git Generator**: Dynamic application discovery and creation based on your Git repository's directory structure.
    
*   **Image Updater**: Automating the flow from container registry to Git by updating image tags automatically.
    
*   **Monitoring**: Configurations for tracking ArgoCD controller health and performance metrics.
    
*   **Multi-Cluster**: Strategies for orchestrating deployments across disparate Kubernetes environments.
    

🛠 Required Configuration
-------------------------

> \[!IMPORTANT\]
> 
> **Update the Cluster Server URL**
> 
> Before applying these manifests, you must replace the hardcoded server IP (https://172.31.19.178:33893) with your own cluster's API server URL.

1.  Run argocd cluster list to see your active server addresses.
    
2.  **Files to update**:
    
    *   declarative\_approach/online\_shop/online\_shop\_app.yml
        
    *   app\_of\_apps/apps/apache\_app.yml
        
    *   app\_of\_apps/apps/nginx\_app.yml
        
    *   app\_of\_apps/apps/online\_shop\_app.yml
        

✍️ My Learning Roadmap
----------------------

I am currently using this repository to:

*   \[x\] Implement the **Declarative Approach** for standardizing deployments.
    
*   \[x\] Configure the **App-of-Apps** pattern for centralized management.
    
*   \[ \] Refine **ApplicationSets** to handle environment-specific overrides.
    
*   \[ \] Explore **Auto-healing** and **Prune** capabilities to prevent manual drift.
    

🤝 Acknowledgments
------------------

Special thanks to the mentors who provided the foundational knowledge for these demos:

*   **TrainWithShubham (TWS)**
    
*   **Amitabh DevOps**
    

_This repo is a work in progress as I continue to learn and update the manifests according to my local environment needs._
