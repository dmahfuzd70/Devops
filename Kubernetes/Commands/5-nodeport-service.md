Create & Display
----------------
      kubectl create -f 4-deployment.yaml
      
      kubectl create -f 5-nodeport-service.yaml
      
      kubectl get service -l app=nginx-app
      
      kubectl get po -o wide
      
Describe
--------
      kubectl describe svc my-service
      
 
Accessing using Pod IP
----------------------
      kubectl get po -o wide
      
      curl http://pod_ip
      
Accessing using Service IP
--------------------------
      kubectl get svc -l app=nginx-app
      
      curl http://service_ip
      
      kubectl get po -o wide
      
      
Cleanup
-------
      kubectl delete svc my-service
      
      kubectl get pods 
      
      
