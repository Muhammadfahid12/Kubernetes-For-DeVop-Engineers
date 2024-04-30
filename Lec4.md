### Worker Node

# kublet: 
        Main service on the node. connect between Master and Node(worker) and ensurring that the pods and their containers are healthy and running in the desired state.
        also reports health of host running to the Master.


# Kube-Proxy:
            A proxy service runs on each worker node to deal with individual host subnetting and expose services to the external world. It performs request forwarding to the correct pods/containers across the various isolated networks in a cluster

# Kubectl:
            Command Line Tool interacts with kube-apiserver and send commands to the master node. Each command is converted to API call.


    ![kubernetes ](images/k8s-big-picture.png)