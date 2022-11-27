common commands
===============
# docker
-- to build with tag
+ docker build -t username/repo:0.0.1 .

-- run image with detached mode
+ docker run -d [imageid/imagetag]

-- after running see the logs
+ docker logs [containerid]

-- see all running processes
+ docker ps

-- log into shell of container
+ docker exec -it [containerid] sh

-- run the docker image and execute command
+ docker run -it [image] sh

-- push to docker hub
+ docker push [imagetag]  should be like byorn/name which should also exist as a repository in docker hub

# kubernetes
-- view pods and deployhments
+ kubectl get pods
+ kubectl get deployments
+ kubectl describe pod [podname]
+ kubectl describe deployment [deploymemntname
+ kubectl delete pod [podname]

-- view logs of a pod
+ kubectl logs [podname]

--log into a container pod
+ kubectl exec -it [podname] sh

-- run a deployment or pod
+ kubectl apply -f [filename.yml]

-- rolling out a deployment
+ kubectl rollout restart deployment [deployment-name]

