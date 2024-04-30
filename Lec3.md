## K8s Master Node Components

# Api Server:

                Primary Component and responsible for orchestrating all operations (scaling, updates and so on) in the cluster. It also acts as gateway to the cluster. It must be accessible from clients from outside the cluster with cluster integrations with CLI and GUI.

# Controller Manager:

                    Engine that runs the control loops, create prods, watches the state
                    of cluster.make changes to drive status toward the desired state.

# Replication Controller:

                    Ensures that specific number of pod replicas are running at one time. made sure that pod is up and running.

# Node Controller:

                    master component which manage various aspects of nodes.

# Scheduler:

                Identify the right node to place a container on based resource limitations or guarantees, taints , tolerations and affinity/ anti-affinity
                role.

# etcd cluster:

                etcd database stores the state of the cluster, incuding node and work laod information in key/value format.

# Add-ons:

            DNS: All k8s clusters should have cluster DNS. DNS in Kubernetes clusters facilitates service discovery, dynamic scaling, and load balancing, improving the efficiency and reliability of communication between components.
