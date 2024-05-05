# Services:
            Enable communication within and outside of a Node
            It has three types

**NodePort**:   Service makes an internal pod accessible on the port on the node. 

**TargetPort**: Pod port on which web server is actually running.This is Service forward request to.

**Port**: Port on the service. server has its own IP address that is called Cluster IP of servcie.

**Nodeport**: Port of the node, where service send the request from the TargetPort.it's range is 30000 t0 32767. 
 
 **Cluster IP**: Service creates an virtual IP inside cluster to enable communication between different services. For Example, Set of Frontend server to a set of backend server

 **Load Balancer**: service provisions load balancer for our application in supported cloud providers.For example, Distribute load across the different web servers in frontend tier.