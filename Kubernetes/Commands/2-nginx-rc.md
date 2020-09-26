Create Replication Controller
------------------------------
    $kubectl create -f nginx-rc.yaml
  
Get pods information
--------------------
    $kubectl get pods
    
How get specific pod when run many pods in cluster
-------------------------------------------------
    $kubectl get po -l app=nginx-app


Details about Replication Controller
------------------------------------
    $kubectl describe rc nginx-rc
    

Use Case
---------

Replication Controller - Node Fail

    $kubectl get po -o wide
    
    $kubectl get nodes
    
Replication Controller - Scalling up

    $kubectl scale rc nginx-rc --replicas=5
    
    $kubectl get rc nginx-rc
    
    $kubectl get po -o wide
    
Replication controller - Scalling down
    
    $kubectl scale rc nginx-rc --replicas=3
    
    $kubectl get rc nginx-rc
    
    $kubectl get po -o wide
    
Remove Replication Controller
-----------------------------
    $kubectl delete -f nginx-rc.yaml
    
    $kubectl get rc
    
    $kubect get po -l app=nginx-app
