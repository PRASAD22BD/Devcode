# Devcode-Assignment
Build a Dockerfile for deploying a simple Ruby on Rails application with PostgreSQL DB  enabled. Application and DB should run on different containers.
# Step - 1 
DOCKER
Build a Dockerfile for deploying a simple Ruby on Rails application with PostgreSQL DB  enabled. Application and DB should run on different containers.
Examples: Example – I (or) Example - II (or) Example - III (or) Example - IV
Note: You can use any ruby on rails examples or create a new simple rails app to satisfy the requirements
# Step - 2 
KUBERNETES
Build a YAML file for the same application you’ve used in your first step to deploy it on Kubernetes. You can use any local cluster provider such as Minikube or K3d. The deployment of the standalone PostgreSQL pod must use Kubernetes StatefulSet. Additionally, the candidate may use any ingress controller they are comfortable with or a service mesh.
Useful Documentation - https://kubernetes.github.io/ingress-nginx/deploy/
# Step - 3 
ARGOCD 
Deploy ArgoCD to manage the deployment of the previously mentioned application using GitOps. The candidate must create a private GitHub repository to manage the YAML files and for GitOps purposes. All ArgoCD config files must be present in the GitHub repository. The expected files include application.yaml to define the application to deploy, ArgoCD config maps (argocd-cm and argocd-rbac-cm), a config file for/(to add) the private GitHub repository and kubernetes manifest files.
Useful Documentation - https://argo-cd.readthedocs.io/en/stable/
# Step - 4  
TEKTON
Set up Tekton pipelines and the Tekton dashboard. The pipeline should download the source code from the public fork of the sample project (Which you’ve containerized in the first step), build the image, and push it to Docker Hub. The candidate is expected to manually run the pipeline from the Tekton dashboard.
Useful Documentation 
https://tekton.dev/docs/
https://tekton.dev/docs/dashboard/#:~:text=Tekton%20Dashboard%20is%20a%20general,creation%2C%20execution%2C%20and%20completion.
https://hub.tekton.dev/tekton/task/kaniko
