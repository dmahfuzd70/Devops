Create Deployment
-----------------
    $kubectl create -f 4-Deployment.yaml
  
    
Display Deployment
------------------
    $kubectl get deploy -l app=nginx-app   
    
    $kubectl get rs -l app=nginx-app
    
Get pod information
-------------------
    $kubectl get po -l app=nginx-app
    

Details about deployment Controller
------------------------------------
    $kubectl describe deploy nginx-deployment
    

Use Case
---------

Deployment - Update
    Useing kubectl set command
    
    $kubetctl set image deploy nginx-deployment nginx-container=nginx:1.9.1
    
   Using editing command(Editing deployment configuration file in vi editor)
   
    $kubectl edit deploy nginx-deployment
    
   Deployment - Check status 
    
    $kubectl rollout status deployment/nginx-deployment
    
    $kubectl get deploy

Deployment - Rollback

    $kubectl rollout status deployment/nginx-deployment
    
    $kubectl rollout history deployment/nginx-deployment
    
    $kubectl rollout undo deployment/nignx-deployment
    
    $kubectl rollout status deployment/nginx-deployment
    
    
 Deployment - Scale up
 
    $kubectl scale deployment nginx-deployment --replicas=5
    
    $kubectl get deploy
    
    $kubectl get po
    
 Deployment - Scale down
    
    $kubectl scale deployment nginx-deployment --replicas=1
    
    $kubectl get deploy
    
    $kubectl get po -l app=nginx-app
    
Remove Deployment
-----------------------------
    $kubectl delete -f 4-Deployment.yaml
    
  
    $kubect get po -l   app=nginx-app
