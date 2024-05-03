 kubctl run nginx --image=nginx
 kubectl run nginx --image=nginx --dry-run=client -o yaml **to check pre-written yaml file**
 kubectl get pods -o wide 
 kubectl get node
 kubectl describe pod nginx
 kubectl replace -f replicaset-defintion