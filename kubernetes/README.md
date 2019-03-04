1. Install kubectl. More info [here](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

2. Create manager
    ```
    kubectl apply -f deployments/manager.yaml
    kubectl apply -f services/manager.yaml
    ```

3. Create volumes to attach to node deployments 
    ```
    kubectl apply -f volumes/node.yaml
    ```

4. Create nodes
    ```
    kubectl apply -f deployments/node.yaml
    kubectl apply -f services/node.yaml
    ```

    Note:You can edit deployments/node.yaml to change node replication number

