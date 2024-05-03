## K8s Master Node Components

1. **Api Server**:

                Primary Component and responsible for orchestrating all operations (scaling, updates and so on) in the cluster. It also acts as gateway to the cluster. It must be accessible from clients from outside the cluster with cluster integrations with CLI and GUI.Act as Frontend of K8s.

2. **etcd**:

                etcd database stores the state of the cluster, incuding node and work laod information in key/value format.
  

3. **Controller**:
                    Brain behind orchestration. responsible for noticing and responding when node containers or endpoint goes down.They bring decision to bring up new containers in such cases.
                    

4. **Scheduler**:

                Responsible to distributing container to mulitple nodes on based resource limitations or guarantees, taints , tolerations and affinity/ anti-affinity
                role.

