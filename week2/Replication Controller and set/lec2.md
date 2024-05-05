# Kubernetes

In Kubernetes, a Deployment is an object used to manage the rollout and scaling of applications. It provides declarative updates to applications, allowing you to describe the desired state for your application, such as the number of replicas, container images, and resource requirements, without needing to worry about the underlying implementation details.

Here's a brief overview of key features and functionalities of Deployments in Kubernetes:

1. **Declarative Updates**: Deployments allow you to declare the desired state of your application in a YAML or JSON manifest file. Kubernetes then ensures that the actual state matches the desired state, automatically making changes as necessary.

2. **Rolling Updates and Rollbacks**: Deployments support rolling updates, meaning that when you update your application's container image or configuration, Kubernetes will gradually update the Pods to the new version without causing downtime. If an update fails, Deployments support automatic rollback to the previous stable version.

3. **Replica Management**: Deployments manage a set of identical Pods, called replicas, ensuring that the specified number of replicas is always running. If Pods fail or are terminated, Deployments automatically replace them to maintain the desired state.

4. **Scaling**: Deployments support both horizontal and vertical scaling. You can scale the number of replicas up or down based on resource demands, allowing your application to handle varying levels of traffic efficiently.

5. **Self-Healing**: Deployments ensure the high availability of applications by automatically restarting failed Pods and replacing them with healthy ones. This helps in maintaining the desired state and ensuring that the application remains available to users.

Overall, Deployments are a fundamental resource in Kubernetes for managing application lifecycle, ensuring reliability, scalability, and agility in deploying and updating applications in a containerized environment.


# commands:

**create**: kubectl create -f deployment.yml
**to keep record cause of change**: kubectl create -f deployment.yaml --record
**directly update image**: kubectl set image deployment fahad-deployment nginx= 1.18-perl --record
**get**: kubectl get deployments
**update**: kubectl apply -f deployment.yml
**status**: kubectl roll
**rollback**: kubectl rollout undo deployment/fahad-deployment
 rollback will undo changes, but when we check rollout history , a new revision will be show of rollout undo. 