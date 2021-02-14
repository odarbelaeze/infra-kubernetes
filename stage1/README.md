# Stage 1

Now we need to run the workloads for our teams. For that we need to create some
`Deployments` and `Services` that can talk to them.

```bash
kubectl apply --recursive -f deployments
kubectl apply --recursive -f services
```
