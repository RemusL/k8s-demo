# Kubernetes Demo

Stack          | Docker Hub URL
---------------|-----------------------------------------
 MongoDB       | <https://hub.docker.com/_/mongo>
 Mongo Express | <https://hub.docker.com/_/mongo-express>

## Deploy

`kubectl apply -f mongo-db.yaml`

`kubectl apply -f mongo-express.yaml`

## Debugging

`kubectl describe pod mongodb-deployment-xxxxxxxxxx-xxxxx`

`kubectl describe service mongodb-service`

`kubectl logs mongo-express-xxxxxx`

## Test

`minikube service mongo-express-service`
