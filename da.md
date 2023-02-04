# Day 35 Task: Managing Persistent Volumes in Your Deployment
🙌 Kudos to you for conquering ConfigMaps and Secrets in Kubernetes yesterday.

🔥 You're on fire! 🔥

## What are Persistent Volumes in k8s
In Kubernetes, a Persistent Volume (PV) is a piece of storage in the cluster that has been provisioned by an administrator. A Persistent Volume Claim (PVC) is a request for storage by a user. The PVC references the PV, and the PV is bound to a specific node. Read official documentation of [Persistent Volumes](https://kubernetes.io/docs/concepts/storage/persistent-volumes/). 

## Today's tasks:
### Task 1:
Add a Persistent Volume to your Deployment todo app.
- Create a Persistent Volume using a file on your node. [Template]()
- Create a Persistent Volume Claim that references the Persistent Volume. [Template]()
- Update your deployment.yml file to include the Persistent Volume Claim. After Applying pv.yml pvc.yml your deployment file look like this [Template]()
- Apply the updated deployment using the command: `kubectl apply -f deployment.yml`
- Verify that the Persistent Volume has been added to your Deployment by checking the status of the Pods and Persistent Volumes in your cluster. Use this commands `kubectl get pods` ,
`kubectl get pv`
Note : Now You know how to apply any file in k8s

### Task 2:
Accessing data in the Persistent Volume,
- Connect to a Pod in your Deployment using command : `kubectl exec -it <pod-name> -- /bin/bash
`
- Verify that you can access the data stored in the Persistent Volume from within the Pod

Need help with Persistent Volumes? Check out this video for assistance.
Keep up the excellent work🙌💥
