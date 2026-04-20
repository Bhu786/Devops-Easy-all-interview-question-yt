docker scerario based interview question 

## scerario 1
u have a docker container running a web server , but u need to update the application code inside it .
==>1. stop the running conainer using " docker stop"
  2.  pull the latest version of the docker iamge with updated code using " docker pull"
  3.  run a new conatiner with the updated iamge , ensuring to map volumes and ports using " docker run "
  4.  verify the new container is running correctly .


how would u approach this task?

==> we will create container iamge and deploy to the server.


## 2
your team is deploying a microservices architecture using docker containers, 
how would u orchestrate and mange these containers effectively ?

==> we can use k8s 

## 3
you have encounterd a problem where a docker container keeps crashing without any clear error message 
how would u trobleshoot and diagnose this issues?

==> dokcer logs or 

## 4
your team needs to share data b/w docker containers how would u accomplish this while maintaing isolation b/w the containers?

==>

##5 u need to ensure that your docker conatiners are secure and compliant with comapny policies .
what security best practies would u implement ?

==>  


# k8s 

your company is migrating its monolithic app to microservices architecture on k8s , how would u plan and excecute this migration ?
1. Assess the monolithic application to identify microservices.
2. Define container images and Kubernetes deployment configurations.
3. Set up a Kubernetes cluster on-premises or using a cloud provider.
4. Deploy microservices to the cluster with proper networking.
5. Implement monitoring and logging solutions.
6. Decompose the monolithic app into microservices gradually.


u have a stateful applications that requires persistent storage in k8s . how would u configure persistent storage for this application ?

==> we can use statefulset

1. Define PersistentVolume (PV) and PersistentVolumeClaim (PVC) in YAML.
2. Choose an appropriate storage class.
3. Specify access mode, capacity, and other parameters in PVC.
4. Attach PVC to pods in their YAML manifests.
5. Deploy pods to Kubernetes cluster, ensuring access to persistent storage.

u r experiencing performance issues with your k8s cluster . how would u diagnose and resolve thes issues?

1. Monitor resource utilization: CPU, memory, disk.
2. Use Kubernetes dashboard or monitoring tools.
I
3. Check logs of individual pods for errors.
4. Scale up cluster by adding more worker nodes if needed.
5. Optimize resource requests and limits for pods.
6. Implement horizontal pod autoscaling. M

u need to deploy a k8s application across multiple environmnet (dev,staging , production ) with diff configutation .
how would u manage environment-specific configuration in k8s?

1. Use ConfigMaps to store environment-specific config data.
2. Create separate ConfigMaps for each environment.
3. Reference ConfigMaps in pod deployment configs using env variables or volume mounts.
4. Use Kubernetes namespaces to isolate resources.
5. Utilize tools like Helm for templating and managing manifests.


your tean wants to implement rolling updates for a k8s deployment to minimize downtime during applicationo upgrades. how would u achieve this ?

1. Define a new version of the container image.
2. Update the deployment configuration to use the new image.
3. Set deployment strategy to "RollingUpdate".
4. Specify maxSurge and maxUnavailable parameters.
5. Apply updated deployment config to the cluster.
6. Monitor rollout progress and rollback if needed.





























