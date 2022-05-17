# k8s
k8s hands on notes
## Minikube 

### Installing

The official documentation is available here (https://minikube.sigs.k8s.io/docs/start/)

```
brew install minikube
```

Start docker:

```
minikube start --driver docker
```

If everything was propperly installed:

```
minikube status
```

Should print:

```
minikube
type: Control Plane
host: Running
kubelet: Running
apiserver: Running
kubeconfig: Configured
```

## Kubeclt

### Commands

Display nodes:

```
kubectl get node
kubectl get pod 
```
#### Create config and secret file:

```
kubectl apply -f mongo-config.yaml # takes a file and creates whatever was configured inside
```
#### Intract with kubectl cluster

```
kubectl get all
kubectl get configmap
kubectl get secret
kubectl --help # general help 
kubectl get --help # Help of one option
kubectl describe service webapp-service # details of the service

kubectl logs [name of the pod] # check logs
kubectl logs [name of the pod] -f # to stream the logs

kubectl get node -o wide # Gives you the internal IP
```

## Project 

* Docker image of the web-app (https://hub.docker.com/repository/docker/nanajanashia/k8s-demo-app)
* Docker image of mongobd (https://hub.docker.com/_/mongo)
* Kubernetes offical documentation (https://kubernetes.io/docs/home/)
