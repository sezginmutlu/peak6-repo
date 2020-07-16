1 - Clone the repo, follow the steps and you need a kubernetes cluster to deploy the following application.

2 - Given the attached app.py, docker file created and using the following command `docker build -t sezginmutlu6/peak6:latest app/` docker image is built.

3 - Using the `docker push sezginmutlu6/peak6:latest` docker image is pushed to the docker registry.

4 - Created `peak6-all.yaml` manifests.

5 - I have the domanin name as `sezginmutlu.com` through AWS. 

6 - In AWS, I created an A record pointing to the ingress IP address `http://34.96.117.132/` and set the name to `http://peak6.sezginmutlu.com/`.

7 - You can use the `peak6.sezginmutlu.com` too see the application.

8 - GIT-repo: https://github.com/sezginmutlu/peak6-repo

  
