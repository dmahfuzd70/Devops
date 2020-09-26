Create ReplicaSet Controller
------------------------------
    $kubectl create -f nginx-rs.yaml
  
Get pods information
--------------------
    $kubectl get pods
    
How get specific pod when run many pods in cluster
-------------------------------------------------
    $kubectl get po -l tier=frontend
    
    $kubectl get rs nginx-rs o wide

Details about ReplicaSet Controller
------------------------------------
    $kubectl describe rc nginx-rs
    

Use Case
---------

ReplicaSet Controller - Node Fail

    $kubectl get po -o wide
    
    $kubectl get nodes
    
    $kubectl get po -o wide
    
ReplicaSet - Scalling up

    $kubectl scale rc nginx-rs --replicas=5
    
    $kubectl get rc nginx-rs
    
    $kubectl get po -o wide
    
ReplicaSet - Scalling down
    
    $kubectl scale rc nginx-rs --replicas=3
    
    $kubectl get rc nginx-rs
    
    $kubectl get po -o wide
    
Remove ReplicaSet
-----------------------------
    $kubectl delete -f nginx-rs.yaml
    
    $kubectl get rc
    
    $kubect get po -l tier=nginx-app
