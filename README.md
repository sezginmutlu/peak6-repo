1 - Clone the repo, follow the steps and you need a kubernetes cluster to deploy the following application.

2 - Given the attached app.py, docker file created and using the following command `docker build -t sezginmutlu6/peak6:latest app/` docker image is built.

3 - Using the `docker push sezginmutlu6/peak6:latest` docker image is pushed to the docker registry.

4 - Created `peak6-deploy.yaml` & `peak6-ingress.yaml` manifests.

5 - Created a deployment using the `peak6-deploy.yaml` file.

6 - Exposed the deployment as NodePort using the command: `k expose deploy peak6-deploy --name=np-peak6 --type=NodePort --port=80 --target-port=5000`

7 - Using the file `peak6-ingress.yaml` ingress created that uses the service NodePort.

8 - You can use the ingress IP to access the application. 

9 - I have the domanin name as `sezginmutlu.com` through AWS. 

10 - In AWS, I created an A record pointing to the ingress IP address `http://34.96.117.132/` and set the name to `peak6.sezginmutlu.com`.

11 - You can use the `peak6.sezginmutlu.com` too see the application.
