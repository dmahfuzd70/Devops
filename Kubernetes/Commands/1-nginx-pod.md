Create pod
-----------
    $kubectl create -f 1-nginx-pod.yaml
    
Verify the pod is running
-------------------------
    $kubectl get pod
    $kubectl get pod -o wide
    $kubectl get pod nginx-pod -o yaml/json
    
Detailes Outpupt
----------------
    $kubectl describe pod nginx-pod
    
Pod - Testing
--------------
    $ping 10.240.120
    
Inside the pod
--------------
    kubectl exec -it nginx-pod --/bin/sh
    
    #hostname
    nginx-pod
    #exit
    
Delete the pod
--------------
    $kubectl delete pod 1-nginx-pod.yaml
