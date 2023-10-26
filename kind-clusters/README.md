# Kind

This direcory contains automation to setup local Kubernetes cluster via
[kind](https://github.com/kubernetes-sigs/kind)

Scripts:

- `get-kind` - pulls given version of kind.
- `manage-clusters` - Create or delete kind cluster.

## Create the cluster

1. Get kind via the provided script:

    ```shell
    cd kind/
    ./get-kind
    ```

1. Create a cluster

    ```shell
    ./manage-clusters create
    ```

    The command above will create a kind clusters.

1. Export kubeconfig file

  ```shell
  export KUBECONFIG="/tmp/flux2-lab-kube-config"
  ```

## Delete the cluster

Delete the cluster and the docker registry with:

```shell
./manage-clusters delete
```
