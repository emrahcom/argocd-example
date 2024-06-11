# ArgoCD example

Run the following after installing `ArgoCD`:

```bash
kubectl apply -f https://raw.githubusercontent.com/emrahcom/argocd-example/main/application.yaml

kubectl get namespaces
kubectl -n argocd-example get pods
```
