This YAML file create pod

pod is smallest unit in kubernetes
It run one container

The pod name is pod-week-11-exam
Inside pod there is one container with name image-week-11-exam

The container use docker image
yakov234/week_11_exam:v1

The application inside container listen on port 8080
containerPort 8080 only tell kubernetes what port app use

This pod is needed to run application inside Kubernetes cluster
It allow Kubernetes to start, stop and monitor the container

to run

kubectl apply -f pod.yaml

