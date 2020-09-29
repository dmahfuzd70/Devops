Create & Display
----------------
    kubectl create -f 4-deployment.yaml
    
    kubectl create -f 6-loadBalancer-service.yaml
    
    kubectl get service -l app=nginx-app
   
 Display
 -------
    kubectl get service -l app=ginx-app
    
    kubectl describe service my-service
    
Accessing using LoadBalancer IP
-------------------------------
    kubectl describe service my-service | grep Load
    
Cleanup
-------

    kubectl delete service
    
    kebectl get pods
    
