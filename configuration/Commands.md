## Required Commands

1. Apply Taint to a Node
```shell
kubectl taint node <node-name> <key>=<value>:<taint-effect>
```
In this case, run the following command to attach a taint to the worker node:
```shell
kubectl taint node kubernetes-lab-m02 group=nginx-app:NoSchedule
```
2. Add Label to a Node (Use in Node Selectors):
```shell
kubectl label nodes <node-name> <key>=<value>
```