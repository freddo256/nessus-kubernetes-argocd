# Nessus-Kubernetes-ArgoCD
These Kubernetes manifests are used to deploy the nessus Docker image onto a Kubernetes server.
The ArgoCD manifest can be used to do the same in an ArgoCD system.

Remember to change the credentials and use an activation code.
Change the service type if you do not use a load balancer.

## Helm
If you want to use Helm that is possible. Use the following repository URL: `https://freddo256.github.io/nessus-kubernetes-argocd/helm/charts`.
1. `helm repo add nessus https://freddo256.github.io/nessus-kubernetes-argocd/helm/charts` to add the repo.
2. `helm repo update` to update the charts in the repository.
3. `helm search repo nessus` to list the repository.
4. `helm install --values helm/values.yaml nessus nessus/nessus` to deploy the nessus chart.