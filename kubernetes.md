# Important Commands: Kubernetes
---

To check the pods in namespace
```
kubctl get pods -n <name-space name>
kubctl get pods -n micro-service
```

To go inside pod
```
kubctl exec -it <pod-name> sh -n <name-space name>
kubctl exec -it kafka-0 sh -n kafka
```

To check logs from pod
```
kubctl logs <pod-name> -n <name-space name>
kubctl logs abc-2kh -n micro-service
```

To delete pod
```
kubctl delete pod <pod-name> -n <name-space name>
kubctl delete pod abc-2kh -n micro-service
```
