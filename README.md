# ArgoCD example

Run the following after installing `ArgoCD`:

```bash
kubectl apply -f https://raw.githubusercontent.com/emrahcom/argocd-example/main/myproject.yaml
kubectl apply -f https://raw.githubusercontent.com/emrahcom/argocd-example/main/application.yaml

kubectl get namespaces
kubectl -n argocd get appprojects
kubectl -n argocd get applications
kubectl -n argocd-example get pods
```

Removing:

```bash
kubectl delete -f https://raw.githubusercontent.com/emrahcom/argocd-example/main/application.yaml
kubectl delete -f https://raw.githubusercontent.com/emrahcom/argocd-example/main/myproject.yaml
kubectl -n argocd-example delete deployment postgres

kubectl -n argocd-example get all

#kubectl delete namespace argocd-example
kubectl get namespaces
```
