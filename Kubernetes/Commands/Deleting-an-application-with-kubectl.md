Deleting an application with kubectl
------------------------------------
First, use kubectl get all to list all applications and services on the cluster.

      $ kubectl get all
      NAME                                    READY     STATUS    RESTARTS   AGE
      po/simple-deployment-3220091887-070cw   1/1       Running   0          7m
      po/simple-deployment-3220091887-h293v   1/1       Running   0          7m
      po/simple-deployment-3220091887-s4szh   1/1       Running   0          7m

      NAME                 CLUSTER-IP    EXTERNAL-IP   PORT(S)        AGE
      svc/kubernetes       10.3.0.1      <none>        443/TCP        1h
      svc/simple-service   10.3.217.22   <pending>     80:32739/TCP   37m

      NAME                       DESIRED   CURRENT   UP-TO-DATE   AVAILABLE   AGE
      deploy/simple-deployment   3         3         3            3           37m

      NAME                              DESIRED   CURRENT   READY     AGE
      rs/simple-deployment-3126793206   0         0         0         37m
      rs/simple-deployment-3220091887   3         3         3         7m

Next, delete the simple app's Deployment and Service using kubectl delete:

      $ kubectl delete deploy/simple-deployment svc/simple-service
      deployment "simple-deployment" deleted
      service "simple-service" deleted
