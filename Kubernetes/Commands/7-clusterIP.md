Display
-------
    kubectl get po -l tier=backend
    
    kubectl get po -l tier=frontend
    
    kubectl get svc -l tier=backend
    
    kubectl get svc -l tier=frontend
    
Accessing Guestbook app using Node IP
-------------------------------------
    kubectl get no -o w
    
    kubectl get svc -l tier=frontend
