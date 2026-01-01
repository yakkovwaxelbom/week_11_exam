This YAML file create  service to kubernetes

service is used to expose pod network

service name is service-week-11-exam
It select Pods with label app=web

service type is NodePort.
NodePort allow access to the app from outside cluster

port 8080 is the service port
targetPort 8080 is the port inside the container like port of docker 8080:8080


Without service pod is not reachable

to run

kubectl apply -f service.yaml

and

minikube service service-week-11-exam

