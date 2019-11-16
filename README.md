# Switch to the k8s branch of this repo if you want to go for Kubernetes...

# K8s cheat sheat
https://kubernetes.io/docs/reference/kubectl/cheatsheet/

## Updating the particular image:

kubectl set image deployment/client-deployment client=vladimir050486/multi-client:v6

## Start minikube

## Minikube ip

## Get into the minikube vm docker ps:

eval $(minikube docker-env)

docker ps 

## Apply chenages:

kubectl apply -f k8s

## Enable ingress:

minikube addons enable ingress

## Add password as a secret;

kubectl create secret generic pgpassword --from-literal PGPASSWORD=admin 

## List secrets;

kubectl get secrets

## Check ingress:

kubectl get svc -n ingress-nginx  

## Check persistent volumes:

kubectl get pv

kubectl describe storageclass  

## Check persistent volumes claim:

kubectl get pvc

kubectl describe storageclass  

## Logging particular pod:

kubectl logs server-deployment-58dc7785c8-c4nd6

## Delete kube service:

kubectl delete service client-node-port  

## Skaffold
Used for watch mode of react client, working HMR with k8s

skaffold.dev