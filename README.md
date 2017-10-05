# redis-cluster-k8s

[Redis cluster] on [Kubernetes].


# How to run

Just enter the following command.

```
$ kubectl create -f redis-cluster/
```

You can clean up.

```
$ kubectl delete -f redis-cluster/
```


# YAML Files

|Name                 |Kind                |Description                               |
|:--------------------|:-------------------|:-----------------------------------------|
|redis-configmap.yml  |ConfigMap           |The contents of redis.conf                |
|redis-endpoint.yml   |Service             |An endpoint of redis cluster.             |
|redis-node-1.yml     |Deployment, Service |Node1                                     |
|redis-node-1.yml     |Deployment, Service |Node2                                     |
|redis-node-1.yml     |Deployment, Service |Node3                                     |
|redis-node-1.yml     |Deployment, Service |Node4                                     |
|redis-node-1.yml     |Deployment, Service |Node5                                     |
|redis-node-1.yml     |Deployment, Service |Node6                                     |
|redis-node-join.yml  |Job                 |A job to join all nodes to the cluster.   |


[Kubernetes]:https://kubernetes.io/
[Redis cluster]:https://redis.io/topics/cluster-tutorial
