# Namespace

Stack          | Docker Hub URL
---------------|-----------------------------------------
 MongoDB       | <https://hub.docker.com/_/mongo>
 Mongo Express | <https://hub.docker.com/_/mongo-express>

## Deploy

`kubectl apply -f mongo-ns.yaml` or `kubectl create namespace mongo`

`kubectl apply -f mongo-db.yaml`

`kubectl apply -f mongo-express.yaml`

## Debugging

`kubectl describe pod mongodb-deployment-xxxxxxxxxx-xxxxx -n mongo`

`kubectl describe service mongodb-service -n mongo`

`kubectl logs mongo-express-xxxxxxxxxx-xxxxx -n mongo`

## Expose

`minikube addons enable ingress`

Get _[minikube ip]_ with `minikube ip`.

Add `[minikube ip]  mongo-express.ro` into **hosts** file.

Browse [https://mongo-express.ro](https://mongo-express.ro)
