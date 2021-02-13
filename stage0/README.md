# Stage 0

First we need to create a cluster, using our provider. Then download and add our config
file to the appropriate environment variable.

```bash
export KUBECONFIG=$HOME/Downloads/demo-kubeconfig.yaml
```

The kubeconfig file should have strict permissions just like your ssh keys.

```bash
chmod 600 $KUBECONFIG
```

You can check that your cluster has been provisioned with.

```bash
kubectl get nodes
```

Finally we'll create a namespace for our demo resources.

```bash
kubectl apply -f namespaces/demo.yml
```
