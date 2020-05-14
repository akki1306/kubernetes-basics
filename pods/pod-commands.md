#Useful pod commands

| Command Description   |Command|
|----------|-------------|
| Get all pods |  kubectl get pods |
| Get all pods wide output |   kubectl get pods -o wide  |
| Get all pods json output | kubectl get pods -o json |
| Get all pods yaml outpu / kubectl get pods -o yaml |
| Describe pod | kubectl describe pod <pod-name> |
| Describe pod with file instead of name | kubectl describe -f <relative-file-path> |
| Executing command inside a running container in pod | kubectl exec db -- ps aux |
| Executing command inside container with interactive -i terminal -t | kubectl exec -it <pod-name> -c <container-name> <command> | 
| Get logs for a pod | kubectl logs <pod-name> |
| JSON Path to retrieve only names of containers from the JSON output of describe pod command | kubectl get -f pod/go-demo-2.yml -o jsonpath="{.spec.containers[*].name}" |
|