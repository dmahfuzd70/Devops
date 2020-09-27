Create ReplicaSet Controller
------------------------------
    $kubectl create -f 3-frontend-rs.yaml
  
Get pods information
--------------------
    $kubectl get pods
    
How get specific pod when run many pods in cluster
-------------------------------------------------
    $kubectl get po -l tier=frontend
    
    $kubectl get rs frontend o wide

Details about ReplicaSet Controller
------------------------------------
    $kubectl describe rc frontend
    

Use Case
---------

ReplicaSet Controller - Node Fail

    $kubectl get po -o wide
    
    $kubectl get nodes
    
    $kubectl get po -o wide
    
ReplicaSet - Scalling up

    $kubectl scale rs frontend --replicas=5
    
    $kubectl get rs frontend
    
    $kubectl get po -o wide
    
ReplicaSet - Scalling down
    
    $kubectl scale rc frontend --replicas=3
    
    $kubectl get rc frontend
    
    $kubectl get po -o wide
    
Remove ReplicaSet
-----------------------------
    $kubectl delete -f 3-frontend-rs.yaml
    
    $kubectl get rc
    
    $kubect get po -l tier=frontend
