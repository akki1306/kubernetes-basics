#Useful replica set commands


| Command Description   |Command|
|----------|-------------|
| Get all replica sets |  kubectl get rs |
| Get all replica sets wide output |   kubectl get rs -o wide  |
| Get all replica sets json output | kubectl get rs -o json |
| Get all replica sets yaml output / kubectl get rs -o yaml |
| Describe replica set | kubectl describe rs <rs-name> |
| Describe pod with file instead of name | kubectl describe -f <relative-file-path> |
| Delete Replica set | kubectl delete -f <replica-set-config-file>|
| Update replica set definition | kubectl apply -f <replica-set-config-file> |
| Remove label from a pod. Hyphen at the end | kubectl label <pod-name> <label>- |
| Add label to pod | kubectl label <pod-name> <label-name>=<label-value>|