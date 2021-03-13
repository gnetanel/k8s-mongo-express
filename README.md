# k8s-mongo-express
K8s with mongodb and mongo express
README.txt
apply configuration in this order

kubectl apply -f mongo-configmap.yaml
kubectl apply -f mongo-secret.yaml
kubectl apply -f mongo.yaml
kubectl apply -f mongo-express.yaml

in case running in minikube, to get external mongo express external service external ip, run:
minikube get service  mongo-express-service
as minikube won't create external ip for the external service of mongo express...


