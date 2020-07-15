Clone the repo, follow the steps and you need a kubernetes cluster to deploy the following application.
Given the attached app.py, docker file created and using the following command `docker build -t sezginmutlu6/peak6:latest app/` docker image is built.
Using the `docker push sezginmutlu6/peak6:latest` docker image is pushed to the docker registry.
Created `peak6-deploy.yaml` & `peak6-ingress.yaml` manifests.
Created a deployment using the `peak6-deploy.yaml` file.
Exposed the deployment as NodePort using the command: `k expose deploy peak6-deploy --name=np-peak6 --type=NodePort --port=80 --target-port=5000`
Using the file `peak6-ingress.yaml` ingress created that uses the service NodePort.
You can use the ingress IP to access the application. 
I have the domanin name as `sezginmutlu.com` through AWS. 
In AWS, I created an A record pointing to the ingress IP address and set the name to `peak6.sezginmutlu.com`.
You can use the `peak6.sezginmutlu.com` too see the application.
