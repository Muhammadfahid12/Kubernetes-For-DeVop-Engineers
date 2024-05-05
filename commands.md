 kubctl run nginx --image=nginx
 kubectl run nginx --image=nginx --dry-run=client -o yaml **to check pre-written yaml file**
 kubectl get pods -o wide 
 kubectl get node
 kubectl describe pod nginx
 kubectl replace -f replicaset-defintion
 kubectl edit replicaset replicaset_definition **it will opens up running configuration in text editor snd we can change in running replicaset**